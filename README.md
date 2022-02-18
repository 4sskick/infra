# INFRA

This gonna be folder specific for Infra setup using Docker:

- php:7.4-apache (php bundle on image, composer inside)
- MySql 8.0
- Adminer

# How to's

Make sure you already have Docker on your machine and run well. Check it by typed `docker --version`. Im using version `Docker version 20.10.8, build 3967b7d`, also check for docker compose, type `docker-compose --version`. 

## Setup Folder

Clone this repo on your machine. To make it run well, put this clone inside folder (name_whatever_you_want). Then create another one name with `code`. So on the folder name_whatever_you_want would be 2 folders, `infra` and `code`. Put project you wanna run inside `code` folder. Then you're ready to `docker-compose up -d`. Let it download [image](https://blog.iron.io/what-is-a-docker-image/) for the first time, to make it ready to create [container](https://blog.iron.io/what-is-a-docker-container/). When it finished then your're ready to 