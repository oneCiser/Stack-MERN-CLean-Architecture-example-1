# MERN Clean Architecture: Example 1
The project is an example of implementing clean architecture in the MERN stack.

## Dependencies
- [API rest](https://github.com/oneCiser/Stack-MERN-CLean-Architecture-backend)
- [Frontend](https://github.com/oneCiser/Stack-MERN-CLean-Architecture-front-end)

## How to run the project
### **Docker compose**
To be able to run the project you need to clone it and execute the following commands inside the root folder.

```shell
$ git submodule init
$ git submodule update --remote --merge
```

Then it is necessary to create the **.env** file using the example file attached to the project and execute the following commands.

```shell
$ docker-compose build
$ docker-compose up
```
### **By project**
To run the projects individually you must have access to the following servers.
- [MongoDB](https://www.mongodb.com/)
- [Redis](https://redis.io/)

Then you must run each container individually or each server within the project taking into account the example environment files within each project

## Architecture
![Components diagram](https://raw.githubusercontent.com/oneCiser/Stack-MERN-CLean-Architecture-example-1/master/resources/architecture.svg)

## Test

### **API rest**
To run the tests in the API rest create a **.env.test** file inside the API rest project and execute the following command

```shell
$ docker-compose run --rm apirest npm run test
```
