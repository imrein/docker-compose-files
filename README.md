# Compose files

A collection of some docker-compose files for local testing and learning purposes.

## Quick start example

1. Move inside desired directory:
```bash
cd networking/adguard
```

**Make sure to edit port mappings to your own needs.**

2. Create a `.env` file in the folder and provide the variables or just replace them inside the file.

3. Setup container using docker-compose:
```bash
docker-compose up -d
```

4. Check if docker container is running and volumes/networks are created:
```bash
docker ps
```

```bash
docker volume ls && docker network ls
```

## Troubleshooting
If there are any issues or the container is not starting, I would check the docker logs to see if there is any information there:

```bash
docker-compose logs -f
```
