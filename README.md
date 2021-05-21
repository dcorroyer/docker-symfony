# A Symfony app w/ Docker

### You can create a new app or dockerize your app

## Prerequisites:

If you want to create a new app with docker, skip this part and go to the **Installation** part.

If you use this repository to dockerize your app, you have to create a folder named app and put your app inside the folder:

    mkdir app

In my case when I dockerize an app with the repository, I clone the repository of the app and rename the folder by app:

    git clone git@github.com:**theprofile**/**therepository**
    mv therepository app

## Installation:

You have to launch the **Install** script:

    ./Install

The script will search in your app folder if an app exists, make sure if the prerequisites are good for you.

Now your project is up. GREAT !

## Informations:

When your app is up, you'll have these containers:

    php74-container
    mysql-container
    nginx-container

You can access all your containers with this command:

    docker exec -it **yourcontainer** bash

    OR
    
    docker-compose exec **yourservice** sh

For example, if you want to connect to your php container, you can do this:

    docker exec -it php74-container bash

## Makefile

A Makefile is up to provide some short commands to help you.
