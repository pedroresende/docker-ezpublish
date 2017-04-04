# Docker eZ Publish 5.x

This docker is an exercise to run eZ Publish legacy < 5.0 on docker.
This is composed by 3 containers, 1 for Nginx, 1 for PHP-FPM and another for
MySQL Server.

# Requirements

- docker-sync (https://github.com/EugenMayer/docker-sync/wiki) (MacOS)
- docker (https://www.docker.com/community-edition#/download)
- docker-compose (https://docs.docker.com/compose/install/)

# Run

## Linux

Extract eZ Publish legacy into ezpublish folder

```
$ docker-compose up
```

## MacOS

Extract eZ Publish legacy into ezpublish folder

```
$ docker-sync-stack start
```

In order to access the database

```
mysql -uroot -proot -P3307
```

Open your browser

```
http://localhost:8080/
```

You can change the default variables values on .env file
