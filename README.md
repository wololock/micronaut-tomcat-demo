# Micronaut Tomcat Startup Event Listener Demo

## 1. Build the WAR file

```
./gradlew war
```

## 2. Run the application inside Tomcat docker container

```
docker run -it --rm -p 8888:8080 -v "$(pwd)/build/libs/micronaut-tomcat-0.1.war:/usr/local/tomcat/webapps/micronaut.war" tomcat:9.0
```