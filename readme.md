## Simple REST API

This is for learning purpose. All code contained here are from this Youtube tutorial
Build A CRUD API With Golang - [2021] - For Beginners 
https://www.youtube.com/watch?v=TkbhQQS3m_o

## Getting started
This demonstrates how to implement CRUD operations for a movies application. For simplicity, we will be using a struct as the data source and perform the operations on the struct.

## Steps
1) AEnsure you are in the movies directory then compile the application using `go build`

2) Next, run the application with `go run main.go`

3) Head on to postman and try the following requests

```
//Retrieve all movies
GET http://localhost:8000/movies

//Retrive only one movie
GET http://localhost:8000/movies/1

//Create a new movie
POST http://localhost:8000/movies

Body {
    "isbn": "432678",
    "title": "Dark Matter",
    "director": {
        "firstname": "Chen",
        "lastname": "Shi-zheng"
    }
}

//Update an existing movie
PUT http://localhost:8000/movies/{id}

Body {
    "isbn": "123456",
    "title": "Example Movie",
    "director": {
        "firstname": "John",
        "lastname": "Doe"
    }
}

//Delete an existing movie
DELETE http://localhost:8000/movies/{id}

```