## springboot_mysql
#### Main package
- java:17
- spring boot:3.1.11-SNAPSHOT
- mysql:8
- mongo:7
- ubuntu:24

#### CLI with Dockerfile and compose.xml : duration 150.4s
```
# --project-name is docker container name
~$ docker-compose --project-name team_fastapi_spring up -d --build
-----------
~$ docker-compose build --no-cache
~$ docker-compose --project-name team_fastapi_spring up -d
```

#### setup extionsion of vscode
- Gradle for Java
- SpringBoot Extension Pack
#### samples
- [src\main\java\com\example\co_templates\CoTemplatesApplication.java](src\main\java\com\example\co_templates\CoTemplatesApplication.java)
