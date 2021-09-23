# Docker + Rails Template

Dockerized rails application template. [Documentation](https://docs.docker.com/samples/rails/)

## Includes

- Ruby 3.0
- Rails 6.14
- Postgresql 13.3

## Steps

1. Update config/database.yml with database values (name, user, password)
2. If you need to, update docker-compose.yml with image names

Run docker

```
dc up -d
```

Run server

```
rails server
```

## Commands

Nuke the shit out of docker

```
docker stop $(docker ps -qa) && docker system prune -af --volumes && docker compose up
```

## TODO

- Webpack + React
- Typescript
