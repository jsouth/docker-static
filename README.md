#Docker Static
Serve a static website using docker swarm

## Run the image
docker run -p 8000:80 --name static jsouth/static-site

## Build the image
docker build -t jsouth/static-site:latest .

## Deploy
docker stack deploy --compose-file docker-compose.yml static-site

## View services
docker stack services static-site