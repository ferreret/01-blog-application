## Cosas a tener en cuenta

Tutorial donde he seguido los pasos para dockerizar la aplicación

- https://learndjango.com/tutorials/django-docker-and-postgresql-tutorial



#### Iniciar aplicación y bbdd de forma detached

```sh
docker-compose up -d --build
```

#### Cerrar containers

```sh
docker-compose down
```


### NOTA IMPORTANTE

Las instrucciones a ejecutar de migración, por ejemplo, se hacen de la siguiente manera


```sh
docker-compose exec web python3 manage.py migrate
```

```sh
docker-compose exec web python3 manage.py createsuperuser
```