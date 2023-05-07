# Turboasya Docker and Docker compose example

## Docker

```sh
docker run --rm \
  --publish 8080:8080 \
  -e MYSQL_DSN="root:root@tcp(127.0.0.1:3306)/turboasya" \
  -e STORAGE="disk" \
  -e DISK_PATH="/mnt/data" \
  -v ~/.turboasya-data:/mnt/data \
  ghcr.io/siberianmh/turboasya:latest
```

## Docker Compose

Check the [docker-compose.yaml](./docker-compose.yaml) file, and after that run
the following command.

```sh
docker compose up
```
