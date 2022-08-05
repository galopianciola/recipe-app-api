# recipe-app-api
Recipe API DRF project

### Run tests inside container
```
docker-compose run --rm app sh -c "python manage.py test"
```


### Migrate (waiting for db)
```
docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"
```