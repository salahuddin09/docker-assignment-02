# docker-assignment-02


## Build and Run with Docker Compose
docker-compose up -d --build

## Access the API
Open: http://localhost:8080/api/todos

## Docker Commands Used

| Command                                                           | Purpose                                |
| ----------------------------------------------------------------- | -------------------------------------- |
| `docker build -t salahuddin09/todo-app:1.0 .`                     | Build the app image                    |
| `docker run -d -p 8080:8080 salahuddin09/todo-app:1.0`            | Run app container                      |
| `docker login`                                                    | Login to Docker Hub                    |
| `docker push salahuddin09/todo-app:1.0`                           | Push image to Docker Hub               |
| `docker-compose up -d --build`                                    | Build and run all services             |
| `docker-compose down`                                             | Stop and remove containers and network |
| `docker image ls`                                                 | List images and sizes                  |
| `docker history salahuddin09/todo-app:1.0`                        | View image layers and sizes            |
| `docker inspect <container>`                                      | Inspect container details              |


## Notes

    The app connects to PostgreSQL via Docker Compose network.
    Health checks and resource limits are configured in docker-compose.yml.

# Summary
The app will be reachable on http://localhost:8080/api/todos.
