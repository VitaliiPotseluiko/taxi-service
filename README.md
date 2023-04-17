# Taxi Service
This application implements a taxi service model with the ability to register and authenticate drivers, control access to various data. Such tools as MySQL, Java Servlet API, Apache Tomcat, JDBC API were used in the implementation.
# Features
You can:
- Add and delete drivers
- Add and delete manufacturers
- Add and delete cars
- Display all drivers, cars and manufacturers
- Display your own cars
- Add and delete drivers to certain car
- Authetication
# Structure
 ***The project has 3-Tier Architectur***
1. DAO
  - all database work takes place here (CRUD methods)
2. SERVICE
  - all businece logic takes place here
3. CONTROLLER
  - all communication between the client and the server takes place here
# Technologies
- **Java 11**
- **MySQL**
- **Maven 3.8.0 version**
- **JDBC 4.2 version**
- **MySql 8.0.22 version**
- **Java Servlets 4.0.1 version**
- **Apache Tomcat 9.0.65 version**
- **JSTL 1.2 version**
# How to run
- Clone this repository `https://github.com/VitaliiPotseluiko/taxi-service.git`
- Initialize the database by using SQL script : `src/main/resources/init_db.sql`
- Update fields JDBC_DRIVER, URL, USERNAME, PASSWORD with your database connection information in
  `src/main/java/taxi/util/ConnectionUtil.java`:
![image] (https://user-images.githubusercontent.com/107885859/232590372-62becf5c-ac22-4937-895e-00a8c9cf7a0b.png)
- Buil this project using Maven: `mvn clean install`
- Configure run with Tomcat
# Autors
  Vitalii Potseluiko
