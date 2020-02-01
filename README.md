# run-gui-app-from-container
Example how to run a GUI app from a container

## Execution:

### Using docker compose
docker-compose build

docker-compose up

### Using docker run
docker build .

docker run -d --net=host --env DISPLAY --volume="$XAUTHORITY:/root/.Xauthority:rw" gui-app
