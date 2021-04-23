## Phone Directory Spring Boot app

User can signup to store contacts and perform CRUD operations on records.

Built using:
- JDK 8
- PostgreSQL

## Run project locally
```
	./mvnw spring-boot:run
	
```

## DB Config

To run using local DB, open Postgres console and run:
```       
    CREATE DATABASE phonebook;   
    CREATE USER bookuser WITH password 'password';     
    GRANT ALL privileges ON DATABASE phonebook TO bookuser; 
```
then run this in the project dir
```
   ./mvnw spring-boot:run -Drun.jvmArguments="-Dspring.profiles.active=postgres" -P postgres 
```
Project will run at localhost:9696/phonebook 
