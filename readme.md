# Node "Hello World" Example

This repository is a sample hello-world application written with NodeJS. It's purpose is to help new developers practice Dockerising applications.

## Dockerising the application
1. Select an appropriate base image from the [list of UKHomeOffice base images here](https://github.com/UKHomeOffice/hosting-platform/blob/master/developer-docs/writing_dockerfiles.md)
  1. **IMPORTANT NOTE!! If completing the developer induction please use the image ```node:6.9-alpine```**
2. We recommend the NodeJS onbuild images, but if you want to play with one of the other images to get more practice that's ok too!
3. Follow the instructions to write a Dockerfile
4. Once you have the Dockerfile build and run your docker image and bind it to one of your host ports
5. Show that the application works by loading it in your web browser

## Running the application without Docker

### Pre-requisites
Node version 4+ and npm are required to run this project.

### Running the application
First, checkout this project locally and then follow these steps:

```bash
node server.js
```

## MYSQL demo
Set the following environment vars:

 - DBHOST (mysql host e.g. 127.0.0.1)
 - DBUSER (mysql user e.g. root)
 - DBPASS (mysql pass e.g. root)
 - DBNAME (mysql database e.g. my database)

#### GET http://localhost:4000/table
You should see a table that increases with every request of the timestamp of the request
