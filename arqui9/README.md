# Newsify GUI

## Settings
```sh
$ export NEW_RELIC_LICENSE_KEY="KEY"
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
$ docker-compose scale web=3
$ docker-compose up --force-recreate -d
$ docker-compose logs
```
