# recipe-app-api
Recipe API DRF project

> Todos los comandos con `docker-compose run --rm app sh -c` serán ejecutados dentro del container de `app`, y luego será eliminado (`--rm`)

### Run tests inside container
```
docker-compose run --rm app sh -c "python manage.py test"
```


### Migrate (waiting for db)
```
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"
```


### Make migrations
```
docker-compose run --rm app sh -c "python manage.py makemigrations"
```


### Correct linting
```
docker-compose run --rm app sh -c "python manage.py wait_for_db && flake8"
```

### Docker compose commands
```
docker-compose build
```

```
docker-compose up
```