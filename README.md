# Deployment

### New Relic
To create a monitoring container:
```sh
# Make sure to replace 'SECRET_KEY' with your actual key
docker run -d \
  -v /var/run/docker.sock:/var/run/docker.sock:ro \
  -e NEW_RELIC_LICENSE_KEY=NEW_RELIC_LICENSE_KEY \
  --privileged \
  --pid="host" \
  --net="host" \
  --ipc="host" \
  -v /sys:/sys \
  -v /dev:/dev \
  --restart=always \
  --name newrelic \
  uzyexe/newrelic
```

Or add it to `docker-compose.yml`:
```sh
newrelic:
  extends:
    file: ./../analytics.yml
    service: newrelic
```
