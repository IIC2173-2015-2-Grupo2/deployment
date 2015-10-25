# News API

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
