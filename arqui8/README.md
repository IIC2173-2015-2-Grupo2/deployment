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

### Setup database
Init PostgreSQL database container:
```sh
$ docker-compose up -d db
```
Lets create a database:
```sh
$ docker-compose run db bash
```

Inside our container, log to postgres service:
```sh
$ psql -U postgres
```

Create Database
```sh
CREATE DATABASE newsapi;
```

Exit postgres:
```sh
\q
```

Exit container:
```sh
$ exit
```

### Setup webapp

```sh
# Start containers
$ docker-compose up -d

# See logs
$ docker-compose logs

# Stop
$ docker-compose stop

# To scale
$ docker-compose scale web=3
$ docker-compose up --force-recreate -d
$ docker-compose logs
```
