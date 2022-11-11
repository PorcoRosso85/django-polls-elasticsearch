# Django Polls Application with Haystack and Elasticsearch
Repository with examples for the Medium articles:
 - [Django Polls App with Elasticsearch](https://medium.com/@s.lyapustin/django-polls-app-with-elasticsearch-ffc02b9e79d9)
 - [Elasticsearch Autocomplete for Django](https://medium.com/@s.lyapustin/elasticsearch-autocomplete-for-django-9dffef1d3afb)


## Run project via Docker
  - Install [Docker](https://www.docker.com/products/docker-desktop)
  - Clone repository: `git clone git@github.com:slyapustin/django-polls-elasticsearch.git`
  - Switch to the project directory: `cd django-polls-elasticsearch`
  - Build and run application via Docker: `docker-compose up`
  - Visit http://localhost/
  - Use login `demo` and password `demo` for the [Django Admin](http://localhost/admin) page


## What we do before when we 'compose up'
Please follow commit "https://github.com/PorcoRosso85/elasticsearch_django/commit/c45354ac03fe905b1337c4cb162daacfcb293f40"
- Fix error because postgres will search port 5432 at local as default
[ref](https://github.com/docker/awesome-compose/tree/master/official-documentation-samples/django)
[ref](https://stackoverflow.com/questions/23724713/installing-postgresql-within-a-docker-container)
- Fix error because postgres will require environment to connect
[ref](https://qiita.com/takos/items/c04ac2a64d519894ee13)
