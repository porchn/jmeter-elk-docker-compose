# jmeter-elk-docker-compose
docker compose for jmeter3.0(master) and run ELK


### How To Use
```
	sudo docker-compose -p projectName up -d

	docker ps
```

result

```
CONTAINER ID        IMAGE                      COMMAND                  CREATED             STATUS              PORTS                              NAMES
2f23e9c818cd        logstash:latest            "/docker-entrypoint.s"   11 hours ago        Up 42 minutes       0.0.0.0:5000->5000/tcp             projectName_logstash_1
db796b94ac1a        kibana:latest              "/docker-entrypoint.s"   11 hours ago        Up 42 minutes       0.0.0.0:5601->5601/tcp             projectName_kibana_1
c17eed95ab19        elasticsearch:latest       "/docker-entrypoint.s"   11 hours ago        Up 42 minutes       0.0.0.0:9200->9200/tcp, 9300/tcp   projectName_elasticsearch_1
a9f7b98e14a9        porchn/jmeter-3.0-master   "/bin/bash"              11 hours ago        Up 42 minutes       0.0.0.0:60000->60000/tcp           projectName_jmeter_1	
```
