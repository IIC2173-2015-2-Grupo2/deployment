# Analyzer2

## Settings
```sh
$ export NEO4J_USER="neo4j"
$ export NEO4J_PASS="PASS"
$ export NEO4J_HOST="arqui7.ing.puc.cl"
$ export NEO4J_PORT="80"
```

## Start
```sh
# Start containers
$ docker-compose up -d

# See logs
$ docker-compose logs

# Stop
$ docker-compose stop

# To scale
$ docker-compose scale analyzer=2
$ docker-compose up --force-recreate -d
$ docker-compose logs
```
