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
![image](https://user-images.githubusercontent.com/107885859/231518045-09822457-0458-4a05-95be-2468868784d2.png)
- **taxi/** - folder contains all of application's logic
- **controller/** - folder contains all the controllers (servlets) to handle requests.
- **dao/** - folder contains all the Dao classes to perform operations on the DB.
- **ecxeption/** - holds all custom exception classes.
- **lib/** - contains Injector class to perform DI and custom annotations.
- **model/** - contains classes: Driver, Car, Manufacturer.
- **service/** - service layer of the application.
- **util/** - contains utility class for database connection.
- **web.filter/** - contains AuthenticationFilter class that provides authentication control.
- **resources/** - contains init_db.sql that helps to initialize DB before running the application.
- **webapp/** - folder with web resources (presentation layer of the application).
- **WEB-INF/views/** - contains the dynamic web-resources - .jsp files to display the web-pages.
- **web.xml** - file that provides servlet mapping.
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
  `src/main/java/taxi/util/ConnectionUtil.java`
- Buil this project using Maven: `mvn clean install`
- Configure run with Tomcat
# Autors
  Vitalii Potseluiko
