# compose-example-orbit-db-http-api
An example docker compose project for the orbit-db-http-api using certbot, nginx, and go-ipfs


### How To Run ###

```
docker-compose up -d
docker-compose exec certbot sh run.sh
docker-compose restart reverse-proxy
```
