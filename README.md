
## User Manager

User Manager is a sample tiny application that performs CRUD jobs on User Entity via Restful Webservices.

It exposes 3 endpoint as following list :

- GET /api/users (get a list of user)
- POST /api/users (create a user)
- GET /api/users/{cpf} (get one user from the list)

## How to setup
It is a docker based application. Running below command in project's directory builds 2 running containers, UserService and Mysql containers with initial records:

```bash
docker-compose up
```


## How to use
This application is Restful and it follows OpenAPI specification in API documentation. Thanks to SwaggerUI, you can see endpoints documentation in a graphical user interface and try their functionality and see the response. After running the containers, you can access the application links as :

- Application Rest services : http://localhost:8090/api/users
- SwaggerUI : http://localhost:8090/swagger-ui.html


## Test

Tests are written with H2 in-memory database with initial records.
