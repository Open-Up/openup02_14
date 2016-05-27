# Time management

In this (short) practical work, we will use **gitlab** to manage our **ntp** configuration.

## Question 1

Install docker following [https://github.com/sameersbn/docker-gitlab](https://github.com/sameersbn/docker-gitlab), quick start section.

```
wget https://raw.githubusercontent.com/sameersbn/docker-gitlab/master/docker-compose.yml

docker-compose up
```

## Question 2

Create 2 projects : 

 - ntp-server
 - ntp-client

 Clone them on your computer.

## Question 3

Launch your NTP server with : 

```
docker run -ti --entrypoint=/bin/bash monsantoco/min-jessie
```

 - Edit the *server configuration project* so that the server is synchronized with de thebian servers, and restricted to your docker network.
 - Install git on the server 
 - clone the server configuration project
 - Launch NTP

## Question 4

Launch the NTP client with 


```
docker run -ti --entrypoint=/bin/bash monsantoco/min-jessie
```
 - Edit the *client* configuration project so that it uses our server for synchronization
 - Install git on the client
 - Clone the server configuration project

## Question 5

Enable broadcast on the server.

What are the advantages of using Git here ?

