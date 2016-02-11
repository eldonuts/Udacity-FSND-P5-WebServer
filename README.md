#### 1. "The IP address and SSH port so your server can be accessed by the reviewer."

52.36.59.21:2200

#### 2. "The complete URL to your hosted web application."

http://restaurants.donuts.io

#### 3. "Summary of software you installed and configuration changes made."

Software Installed:
- Postgres
- Apache2
- Git
- Pip

Config Changes:
1. Set up new Role/User in postgres and gave it ownership of new database called catalog.
2. Checked that postgres remote connections were disabled (always turned off by default for Ubuntu distributions).
3. Altered my config.py (my app) to connect to postgres database.
4. Altered apache2 config to point at new catalog.wsgi file.
5. Altered apache2 config to add in environment variables (just one for now).
6. Altered catalog.wsgi to import the environment vriables.
7. Altered permissions on certain files and kept some as root in app dir (some needed www-data permissions).
8. Installed requirements with pip and requirments.txt

#### 4. "A list of any third-party resources you made use of to complete this project."

http://flask.pocoo.org/docs/0.10/deploying/mod_wsgi/
http://flask.pocoo.org/snippets/99/
https://www.digitalocean.com/community/tutorials/how-to-secure-postgresql-on-an-ubuntu-vps
http://ericplumb.com/blog/passing-apache-environment-variables-to-django-via-mod_wsgi.html
http://www.postgresql.org/docs/current/static/sql-commands.html
