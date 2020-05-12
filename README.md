# Postgis DB + PgAdmin4

```
rm -rf postgres-data
docker-compose down && docker-compose build && docker-compose up
```

*From pgadmin connect using the ip, not localhost*

```
ipconfig getifaddr en0
```

## Kill previous process

From: https://github.com/docker/compose/issues/4950#issuecomment-398879461

```
docker-compose down
docker rm -fv $(docker ps -aq)
sudo lsof -i -P -n | grep 5432
kill -9 <process id>
```
