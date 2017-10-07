# microservices

```
docker network create reddit
docker volume create reddit_db

docker run -d --network=reddit -v reddit_db:/data/db --network-alias=post_db --network-alias=comment_db mongo:latest
docker run -d --network=reddit --network-alias=post gis23/post:1.0
docker run -d --network=reddit --network-alias=comment gis23/comment:1.0
docker run -d --network=reddit -p 9292:9292 gis23/ui:2.0
```
