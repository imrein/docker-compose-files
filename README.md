# Compose files

A collection of my compose files that I use. The bind mounts need to be adjusted to custom locations.
The data for every container is stored in a volume which will be created when the docker-compose file is used.

## Quick start example

1. Move inside desired directory:
```
cd adguard
```

2. Setup container using docker-compose:
```
docker-compose up -d
```

3. Check if docker container is running and volumes/networks are created:
```
docker ps
```

```
docker volume ls && docker network ls
```

## Troubleshooting
If there are any issues or the container is not starting, I would check the docker logs to see if there is any information there:

```
docker-compose logs -f
```

Or check for individual container logs:
```
docker ps
docker logs traefik
```
