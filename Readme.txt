https://www.youtube.com/watch?v=x7nrGLJLN5U


gradle clean build
gradle docker --info
docker images
docker run -it -p 8082:8080 mycoolapp2

root@BERLIN:/opt/demo-docker-image# docker ps
CONTAINER ID   IMAGE             COMMAND                  CREATED          STATUS          PORTS                                       NAMES
d2af5fd82fdc   mycoolapp2        "java -jar /app.jar"     30 seconds ago   Up 22 seconds                                               distracted_aryabhata
53af593a1c94   sonatype/nexus3   "/opt/sonatype/nexus…"   2 weeks ago      Up 35 minutes   0.0.0.0:8081->8081/tcp, :::8081->8081/tcp   jacek_nexus_1


root@BERLIN:/opt/demo-docker-image# curl --head localhost:8082
HTTP/1.1 404
Content-Type: application/json;charset=UTF-8
Transfer-Encoding: chunked
Date: Mon, 28 Nov 2022 21:16:09 GMT

