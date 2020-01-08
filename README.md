# Docker Apache2 Webserver
Local Apache2 webserver development enviornment and setup using Docker and Docker Compose.

This Docker image uses the following containers:
* php:7.1.20-apache

## Requirements
Make sure you have the latest version of **Docker** and **Docker Compose** installed.

Clone this repository or copy the files from this repository into your new site directory.

## Configuration

### Ini
Edit the php.ini config with `config/php/php.ini`

### VHosts
Edit the vhost config with `config/vhosts/default.conf`

## Installation
Open a terminal and `cd` to the folder that contains `docker-compose.yml` and run:
```
docker-compose up
```

Contains should now be built and running.  
By default the site will be running on `localhost:80`.


## Usage

### Starting Containers
```
docker-compose up -d
```

### Stoping Containers
```
docker-compose stop
```

### Removing Containers
To stop and remove all containers
```
docker-compose down
```
If you need to remove the database volume as well use:
```
docker-compose down -v
```

### Development
Site root directory is the `app` folder