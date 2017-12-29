# microservices

edit `.env.example` file and rename it to `.env`

edit `alertmanager/config.yml.example` file with your webhook uri and chanelname and save it as `alertmanager/config.yml`

run
```
docker-compose up -d
```

check app at http://docker-host:9292

monitoring page at http://docker-host:9090

grafana dashboards at http://docker-host:3000

cadvisor available at http://docker-host:8080
