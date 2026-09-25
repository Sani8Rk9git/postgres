# WORKING WITH DATABASES

- Listing the existing databases
    - from the command line
        - \l (only for command line)
    - ```SELECT datname FROM pg_database;```(write this exactly)

    - from the pgadmin
        - select the database
        - click tools --> query tool
        - now we can write and execute query
        - ```SELECT datname FROM pg\_database;```
        - execute it


- SQL is case-insensitive
- semi-colon ends the query
    - if our query is very large, we can write it in multiple lines
    - when the query ends, just put the semi-colon

- the psql and pgadmin both are interface that are connected to the backend of postgres
    - if we write the query in any interface the changes are updated in both
    - in the pgadmin, just refresh
    - To execute queries in the query tool, after writing the query, select them and then run.


### Creating a new database

- ```CREATE DATABASE <name>;```
- in the pgadmin, just right click on the database and choose create database
- same right click and do refresh

- to change the database(means we are currently in a database, now I want to get inside another database)
    - command line
    - ```\c <name>;```
        - name is the database we want to use
    - on pgadmin
        - click on the database name
        - open query tool
        - now the query tool and the query we write will be applicable to that database.

### deleting a database

- ```DROP DATABASE <name>;```
    - if the database we want to delete is connected to the server, it will not delete
    - go to pradmin
    - right click on the database
    - disconnect from the server
    - now execute the query
    - also we can choose the delete(force) to force the deletion

