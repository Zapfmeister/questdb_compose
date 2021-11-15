# QuestDB Docker Compose
## _Docker Compose for QuestDB_

This is a docker-compose setup for QuestDB

# Howto

## Quick start
```sh
git clone https://github.com/Zapfmeister/questdb_compose.git
cd questdb_compose
docker-compose up -d
```

## Credentials
Default credentials for postgresql access are:
| Variable | Entry |
| ------ | ------ |
| User | myuser |
| Password | changeme 

You can update the credentials by updating the .env file:
```sh
nano .env
```

## Logging
Configure logging via:
```sh
nano questdb/conf/log.conf
```
Please note that the environment variables set in docker-compose.yml take priority over settings in the configuration files!

## Additional configuration via docker-compose.yml
Further configuration is available via environment variables within the docker-compose.yml file.
The available configuration variables can be found in the QuestDB Variables section. (See Links below)

## Links
| Name | Link |
| ------ | ------ |
| QuestDB Github | https://github.com/questdb/questdb |
| QuestDB Documentation | https://questdb.io/docs/introduction |
| QuestDB Variables | https://questdb.io/docs/reference/configuration |
| QuestDB Docker Hub | https://hub.docker.com/r/questdb/questdb
