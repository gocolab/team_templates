## Big Data Engineer Training Course Lab Template
#### Main package
- JAVA(17)
- Python(3.11)
- spring boot:3.1.1
- mysql:8
- mongo:7
- Fastapi(0.110)

#### setup extionsion of vscode
- Gradle for Java
- SpringBoot Extension Pack

#### connection between docker containers
    ports:
      - 8888:8888  -> jupyter
      - 8000:8000  -> fastapi
      - 8080:8080  -> springboot
  db_mysql_8_202402051308:
    image: mysql:8
    restart: always
    environment:
      MYSQL_ROOT_PASSWORD: cocolang
      MYSQL_LOWER_CASE_TABLE_NAMES: 1      
      MYSQL_DATABASE: cocolang
      MYSQL_USER: cocolang
      MYSQL_PASSWORD: cocolang
    ports:
      - "3306:3306"  
