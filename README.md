# HelloDockerApp
Sample full stack web application that is fully containerized with Docker.

There will be a data volume for persistence of data storage for the database even if the image or container is destroyed.

## Architecture
-------
There will be 4 Docker containers used in this architecture:

1. Web application - Angular front end with a .NET Core service.

2. Web Server - NGINX

3. Database - PostgreSQL server

4. Data volume - persistent data storage for Postgr

```
$ TREE
.
|-- README.md
|-- docker-compose.yml
|-- nginx
|      |-- Dockerfile
|      |-- xxx.conf
|      |-- nginx.conf
|-- postgresql
|      |-- Dockerfile
|-- web
|      |-- Dockerfile
```


## PGADMIN4 Configuration
------------------
http://localhost:5050

### New Server Registration

#### General Tab
* Name = postgres

#### Connection Tab
* Host name/address = postgres
* Port = 5432
* Maintenance database = hellodocker
* Username = postgres
* Password = ********