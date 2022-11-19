# CRUD application

### Technology stack
- Java
- SpringBoot
- MySQL
- Docker
- REST API

### MySQL Image
https://hub.docker.com/_/mysql

### Starting a MySQL instance

`docker run --name movielibrary-mysql -e MSQL_ROOT_PASSWORD=root -d -p 3306:3306 mysql:latest`

### Endpoints

| HTTP Method | URL                              | Description                            |
|-------------|----------------------------------|----------------------------------------|
| GET         | http://localhost:8080/           | ROOT page                              |
| GET         | http://localhost:8080/movies     | Get all movies                         |
| GET         | http://localhost:8080/movies/{movieId} | Get movie by id                  |
| POST        | http://localhost:8080/movies | Create new movies                          |
| PUT         | http://localhost:8080/movies/{movieId} | Update movie by id(the whole object)   |
| PATCH       | http://localhost:8080/movies/{movieId} | Update movie by id(part of the object) |
| DELETE      | http://localhost:8080/movies/{movieId} | Delete movie by id                     |


All requests available in Postman collection:
https://www.postman.com/collections/4fe2a8c5f42295aad624