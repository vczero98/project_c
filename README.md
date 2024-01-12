## Running docker

The docker image will be specified in the Dockerfile. This specifies the versions of Node and npm. The `compose.yaml` file is configured to allow access to files local to this project, and not just a copy inside the docker container.

Install and run docker locally. To start the container, run:

```
docker compose up
```

Then, to attach to the terminal, run:

```
docker exec -it CONTAINER_NAME_FROM_COMPOSE_YAML sh
```

That will attach you to the terminal of the container, running the specified version of Node and npm. This is where you'll run `npm install` etc.
