# INSTALLING POSTGRESQL

- google : search download PostgreSQL	
- https://www.postgresql.org/
- DOWNLOAD
- windows
- download the installer
- latest version click download icon
- installer gets installed
- open installer
- next ..
- **set password and note it down**
- finish
- **default username is postgres**

### To use PostgreSQL

- search pgAdmin in the window search
    - open it
    - pgAdmin is a UI using which we can write our queries

- we also get a command line tool
    - we can use the command line to write the queries and access the database
    - search sqlshell (psql)
    - open
    - enter to keep the default
    - enter password
    - command line appears

### now we can write our query in the command line

- to check existing databases in postgres
    - ```\list```
    - enter

- to clear the screen
    - ```\! cls```
    - enter

### SQL

- To create a database
    - ```CREATE DATABASE <database_name>;```

- after creating the database from the command line go to pgAdmin dashboard
    - click server
    - enter password
    - server gets connected

- see that the created database shows there


### can run the psql from the command prompt of the windows
- go to c drive -> program files -> PostgreSQL -> 18 -> bin
- copy the path and set to environment variables
- open command prompt
- ```write: psql -U postgres```
- enter password
- now you can use 

