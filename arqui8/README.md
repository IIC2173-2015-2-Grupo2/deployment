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
$ docker-compose rm web1 web2 ...
$ docker pull iic2173grupo2/news-api
$ docker-compose up -d --no-deps web1 web2 ...
$ docker-compose restart nginx
```
