## General

NOTE: Do not try this solution unless your machines has ample ram available. I have been successful uploading the Yelp database file after allocating 14GB of ram to the Docker VM. OOM crashes are likely if less ram is used.

This repo is a simple docker-compose file which:
1) Starts a ``postgreSQL`` server on port ``5432``
2) Starts an ``Adminer`` database management service on port ``8080`` with a custom php config to allow massive file uploads

## Dependencies

Docker
Docker-compose

## Usage

### Startup
1) Run ``docker-compose -f stack.yml up``
2) Go to ``http://localhost:8080`` in your favorite browser
3) Enter in your database credentials
    * System: postgreSQL
    * Host: use your computer's local IP. Should be something like ``192.168.20.1``
    * Username: postgres
    * Password: test

### Import Yelp Database
1) Make sure database server is running and login to adminer
2) On the left hand side of the screen you should see an import link
