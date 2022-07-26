# Dockerize Django Airline

## Introduction

Dockerize Django Airline is an example of how Django and Postgres may be run under Docker. The Django app here is a simple app for keeping track of flights and passengers.

Using the approach in this project, neither Python, pip, Postgres, nor Django is necessary to install locally on the computer. Everything runs inside of Docker. All that is necessary is Docker. The `docker-compose.yml` file will use `volumes` to create a copy of the Django project and the Postgres data in your local directory, where your `docker-compose.yml` file is stored. Any changes you do in those directories will be reflected in the Django app that is running in a Docker container.

## Requirements

Docker.

## How to use

You should now be able to run the Django Flight app on URL `http://localhost:8000/flights` with the command:

```
docker-compose up
```

### Shutting down the Django development server

Either run

```
docker-compose down
```

in a new terminal window, under the directory where you have your `docker-compose.yml` file.

ALternatively, press `Ctrl+C`.

## Acknowledgements

The project is created as part of Harvard's CS50 Web Programming with Python and JavaScript course. The docker implementation is an adaption of the official Docker documentation, which you can read [here](https://docs.docker.com/samples/django/)

## Intellectual Property Rights

MIT
