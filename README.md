# Taxi Service
This project is taxy service's imitation which uses Servlets and SQL.
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
- taxi/ - folder contains all of application's logic
- controller/ - folder contains all the controllers (servlets) to handle requests.
- dao/ - folder contains all the Dao classes to perform operations on the DB.
- ecxeption/ - holds all custom exception classes.
- lib/ - contains Injector class to perform DI and custom annotations.
- model/ - contains classes: Driver, Car, Manufacturer.
- service/ - service layer of the application.
- util/ - contains utility class for database connection.
- web.filter/ - contains AuthenticationFilter class that provides authentication control.
- resources/ - contains init_db.sql that helps to initialize DB before running the application.
- webapp/ - folder with web resources (presentation layer of the application).
- WEB-INF/views/ - contains the dynamic web-resources - .jsp files to display the web-pages.
- web.xml - file that provides servlet mapping.
# Technologies
- Java
- JDBC for relational DB connection.
- Java Servlet + JSP to handle requests and display dynamic web-pages.
- Deployed using Apache Tomcat running om Amazon AWS EC2 instance and RDS MySQL database.
# How to run
- Clone this repository
- Run the SQL script which located in path src/main/resources/init_db.sql to initialize database
- Buil this project using Maven: mvn clean install
- Deploy the war file to the servlet container, for example Tomcat
# Autors
  Vitalii Potseluiko
