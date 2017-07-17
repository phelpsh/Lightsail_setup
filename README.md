# Lightsail_setup
Ubuntu Linux setup on Amazon Lightsail

http://34.207.130.121/ port:2200
Application can be found in home directory: http://34.207.130.121/

Linux general:
Created grader user
Generated ssh on local machine
Tested ssh using ubuntu user - ok
Transferred public key to authorized_keys 
Generated grader key and tested, ok -- name is graderKey
Changed ssh port to 2200

Application:
Installed postgresql
Installed apache2
Started apache2
Created postgres_user
Changed to postgres_user: sudo su - postgres_user
Started database: psql my_postgres_db

Installed pyscopg2 for connection to Postgres via Python
Installed Jinja2 templates
Installed python-oauth2client
Fixed database create_engine address for application (thanks to http://www.revsys.com/writings/postgresql/errors.html#cannot-connect-remote)

Helpful resources:
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps -- to deploy a flask application
https://www.digitalocean.com/community/tutorials/how-to-create-remove-manage-tables-in-postgresql-on-a-cloud-server -- to create postgres db

Created file database_setup.py 
Changed my project.py from https://github.com/phelpsh/Catalog-App to __init__.py to start on application initiation
Set up sqlalchemy create_engine connections
Copied over all the css and html files to run the application
Had to change Google API to accept JavaScript origins from http://34.207.130.121/ (thanks to advice from https://stackoverflow.com/questions/16850350/got-origin-mismatch-error-in-google-share-api)
Updated packages

