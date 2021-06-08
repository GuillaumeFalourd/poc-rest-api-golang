# poc-rest-api-golang

## Prerequisites

### Golang

- Go installed
- GOPATH configured

### Dependency

- `go get -u github.com/gorilla/mux`

## Description

POC of a JSON API that will allow users to create, read, update and delete events using [mux](https://github.com/gorilla/mux) (A powerful HTTP router and URL matcher for building Go web servers).

## How to use?

On the repo directory, run: `go run main.go`

### Services

GET: `http://localhost:8080`

POST: `http://localhost:8080/events`

```json
{
    "Id": "2",
    "title": "New event",
    "description": "New event description"
}
```

GET: `http://localhost:8080/events/{id}`

GET: `http://localhost:8080/events`

PATCH: `http://localhost:8080/events/{id}`

```json
{
    "title": "Update event",
    "description": "Update event description"
}
```

DELETE: `http://localhost:8080/events/{id}`
