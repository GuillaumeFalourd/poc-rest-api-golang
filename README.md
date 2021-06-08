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

#### Hello World

GET: `http://localhost:8080`

![hello-world](https://user-images.githubusercontent.com/22433243/121230719-fa359600-c865-11eb-93f4-eeb48f1cf586.png)

#### Create event

POST: `http://localhost:8080/events`

```json
{
    "Id": "2",
    "title": "New event",
    "description": "New event description"
}
```

![create event](https://user-images.githubusercontent.com/22433243/121230734-002b7700-c866-11eb-96d9-8232a54b42ec.png)

#### Get event by ID

GET: `http://localhost:8080/events/{id}` (specific event)

![get event](https://user-images.githubusercontent.com/22433243/121230759-07528500-c866-11eb-95ba-3a40fd2a6463.png)

#### Get all events

GET: `http://localhost:8080/events` (all events)

![all events](https://user-images.githubusercontent.com/22433243/121230781-0d486600-c866-11eb-9f53-424e8529170d.png)

#### Update event

PATCH: `http://localhost:8080/events/{id}`

```json
{
    "title": "Update event",
    "description": "Update event description"
}
```

![update event](https://user-images.githubusercontent.com/22433243/121230798-12a5b080-c866-11eb-835e-5a2212ae4387.png)

#### Delete event

DELETE: `http://localhost:8080/events/{id}`

![delete event](https://user-images.githubusercontent.com/22433243/121230820-1802fb00-c866-11eb-9474-ea4acf3214ad.png)

