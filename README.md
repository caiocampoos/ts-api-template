
# TS-Api-Template
[![Test](https://github.com/caiocampoos/ts-api-template/actions/workflows/test.yml/badge.svg)](https://github.com/caiocampoos/ts-api-template/actions/workflows/test.yml)
[![Deploy to Amazon ECS](https://github.com/caiocampoos/ts-api-template/actions/workflows/deploy.yml/badge.svg)](https://github.com/caiocampoos/ts-api-template/actions/workflows/deploy.yml)

  

###  Summary
This api is built with a modular arquitechture aproach, new functionality is added with new modules that share some of its services and utility, routes are registered in the server as the application develop and validation on the api side is done using JSON.schemas. 

  
  #### Pros 
- Easy to get context for how the application works
- Good for expanding functionality with code cohesion. 
- Better test structure and easy to integrate new services.

#### Cons
- Code base is bigger than other aproachs, less abstraction in favor of code clarity.

### :rocket: Requirements

- Docker 
- Docker-compose (for local development)
- nodejs >=16
  
### :checkered_flag: Getting started


docker-compose up -d --build

### Run development Environment 

```
docker-compose up -d --build

Api is running on:

http://0.0.0.0:3001/docs

```

### Run Integration tests

change .env DB url to test URL, instructions on comments in the .env file


```
docker-compose up -d --build

run tests
npm run test:init

```



### For more information on local tests and db schemas go to [Tests and Schemas](https://github.com/caiocampoos/ts-api-template/blob/main/docs/test-documentation.md)
