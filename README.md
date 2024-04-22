## Big Data Engineer Training Course Lab Template
#### Main package
- JAVA(17)
- Python(3.11)
- spring boot:3.1.1
- mysql:8
- mongo:7
- Fastapi(0.110)

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
