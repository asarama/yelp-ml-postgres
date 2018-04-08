## General

This repo is a simple docker-compose file which:
1) Starts a postgreSQL server on port 5432
2) Starts an Adminer database management service on port 8080

## Dependencies

Docker
Docker-compose

## Usage

Run
```
docker-compose -f stack.yml up
```

Afterward visiting
```
http://localhost:8080
```
Should display Adminer

Set the driver to postgreSQL
Set the location to your computer's local IP example 192.168.20.1
Set the user to postgres
Set the password to test