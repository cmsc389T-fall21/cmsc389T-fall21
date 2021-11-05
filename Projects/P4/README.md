# Project 4 Base Image

The files included in this directory allow you to create a docker image with python and twilio preinstalled. You can create a container by running

```
docker-compose up -d
```

When you want to connect to this container, just run

```
docker-compose run hooks_example bash
```

The docker-compose file should mount your current directory.
