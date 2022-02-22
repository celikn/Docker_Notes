# Docker_Notes

creating postgis docker container
```
docker run --name=postgisdb -d -e POSTGRES_USER=myuser -e POSTGRES_PASS=test123 -e POSTGRES_DBNAME=dbforpostgis -e ALLOW_IP_RANGE=0.0.0.0/0 -p 5439:5432 -v pg_data:/var/lib/postgresql --restart=always kartoza/postgis:latest
```
