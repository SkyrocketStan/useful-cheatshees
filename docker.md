docker-compose up for only certain container
```
docker-compose up -d <service name>
```


Show logs of detached containers
```
docker-compose logs
```


Set some services not start automatically.
```yaml
services:
  client:
    # ...
  db:
    # ...
  npm:
    profiles: ["cli-only"]
    # ...
```
```bash
docker-compose up # start main services, no npm
docker-compose run --rm npm # run npm service
docker-compose --profile cli-only up # start main and all "cli-only" services
```