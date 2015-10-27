# News API

## Settings
```sh
$ export NEO4J_USER="neo4j"
$ export NEO4J_PASS="PASS"
$ export NEO4J_HOST="arqui7.ing.puc.cl"
$ export NEO4J_PORT="80"
$ export SECRET_HASH="SECRET_HASH"
$ export AUTH="ENABLE"
$ export ENVIRONMENT="PRODUCTION"

$ export NEW_RELIC_LICENSE_KEY="KEY"
$ export ANALYTICS_TOKEN="TOKEN"
$ export LOADER_IO_TOKEN="TOKEN"
```

## Start
```sh
# Start containers
$ docker-compose up -d

# See logs
$ docker-compose logs

# Stop
$ docker-compose stop
```

## Upgrade
```sh
$ docker-compose stop web1 web2 ...
$ docker-compose rm --force web1 web2 ...
$ docker pull iic2173grupo2/news-api
$ docker-compose up --force-recreate -d --no-deps nginx web1 web2 ...
```
