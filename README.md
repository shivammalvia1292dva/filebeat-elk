1.) Provide your local log path and run below command(Since we are reading log from console filebeat is not required to be installed).

2.) docker run -d --name=filebeat --user=root --network="host" --volume="D:/projects/spring-boot-setup/currency-exchange-service/logs:/logs" --volume="D:/projects/filebeat-elk/filebeat.docker.yml:/usr/share/filebeat/filebeat.yml:ro" docker.elastic.co/beats/filebeat:7.10.2 filebeat -e --strict.perms=false
