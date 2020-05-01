# First spring boot application

Execute the project using maven:
mvn package && java -jar target/gs-spring-boot-0.1.0.jar

for maven dependency error (handshake error)
delete ~/.m2 directory and re-execute

## table sql:
create database restapi;
create table restapi.user (
id int not null auto_increment,
name varchar(255) not null,
email varchar(255) not null,
primary key (id)
);

ALTER TABLE restapi.user
ADD CONSTRAINT PK_User PRIMARY KEY (id); 