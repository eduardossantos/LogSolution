# LogSolution
Log solution with RabbitMQ, LogStash, ElasticSearch and Kibana

## Releases and Release Notes

##required
Docker and Docker Compose installed.


## How to use
```
git clone https://github.com/eduardossantos/LogSolution.git
docker-compose up
```

## Result

### RabbitMQ
- New and default *virtual host* ```EnterpriseLog``` will be created automatically
- Use **[http://localhost:15672/](http://localhost:15672/)** for management with **User**: ```logUser``` and **Password**: ```logPwd```

### ElasticSearch
- Will be used to storage Log content

### LogStash
- Are configurated to **create** ```ApplicationLog``` *queue* on ```EnterpriseLog``` *virtual host* and listen this queue
- Every message in ```EnterpriseLog/ApplicationLog``` will be send to ```ElasticSearch```

### Kibana
- Was configurated do read ```ElasticSearch```
- Use **[http://localhost:5601/](http://localhost:5601/)** for management Kibana without credentials



### Contacts
Eduardo Santos
eduardo120983@gmail.com
Cell: (21)99758-6868
Linkedin: https://www.linkedin.com/in/eduardo-santos-272a08a1/

