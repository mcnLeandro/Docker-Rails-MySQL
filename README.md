# Docker-Rails-MySQL
This repository was created to quick start Rails development with Docker.

# Getting Started

1. Clone repository
```
$ git clone https://github.com/mcnLeandro/Docker-Rails-MySQL.git {your app name}
```

2. Go to the app, and install the node dependency
```
$ cd {your app name}
$ yarn install -y(or you can just type 'npm install -y')
```

3. Build container
```
$ docker-compose build
```

4. Create DB
```
$ docker-compose run web rake db:create
```
5. Start container

```
$ docker-compose start
```


6. Now, you can see "Yay! You’re on Rails!" in (http://localhost:3000/)


7. This is optional, but if you don't like typing long
`
docker-compose run web rails db:migrate
`
You can follow this
```
$ docker ps (to find container id)
$ docker exec -it <working contaner id > bash
(then you'll see like)
root@a9b19e00552e:/myapp#
```
Now, you can type as normal rails command
```
root@a9b19e00552e:/myapp# rails db:migrate
```

## References(Japanese)

- https://qiita.com/nsy_13/items/9fbc929f173984c30b5d
- https://qiita.com/chisaki0606/items/68e21d9a31f1eaaeac00



# Rails Description

## Ruby version
- 2.6.7
## System dependencies
- node_modules
## Configuration
-
##  Database creation
- MySQL
## Database initialization
-
## How to run the test suite
-
## Services (job queues, cache servers, search engines, etc.)
-
## Deployment instructions
-
