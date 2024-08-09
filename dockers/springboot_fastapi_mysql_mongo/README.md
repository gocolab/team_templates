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
- ports:
  - 8888:8888  -> jupyter
  - 8000:8000  -> fastapi
  - 8080:8080  -> springboot
- db_mysql_8:
  - MYSQL_ROOT_PASSWORD: cocolabhub
  - MYSQL_LOWER_CASE_TABLE_NAMES: 1      
  - MYSQL_DATABASE: cocolabhub
  - MYSQL_USER: cocolabhub
  - MYSQL_PASSWORD: cocolabhub
  - "3306:3306"  
- db_mongodb_7:
  - 27017:27017   
