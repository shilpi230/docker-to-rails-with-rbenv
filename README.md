# Docker to Rails App
Docker mysql, memcached, redis and puma services.

### Build the project
```
docker-compose up
```

### Database config
#### Create database
```
docker-compose run web bundle exec rake db:create
```
#### Create tables
```
docker-compose run web bundle exec rake db:migrate
```
#### Import data test
```
docker-compose run web bundle exec rake db:seed
```