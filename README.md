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
 ### The project has 3-Tier Architectur
1. **DAO**
   - CarDaoImpl - processes car model from DB
   - ManufacturerDaoImpl - processes manufacturer model from DB
   - DriverDaoImpl - processes driver model from DB
2. **SERVICE**
   - CarServiceImpl - processes car's CRUD logic
   - DriverServiceImpl - processes driver's CRUD logic
   - ManufacturerServiceImpl - processes manufacturer's CRUD logic
   - AuthenticationServiceImpl - processes authentication logic
3. **CONTROLLER**
   - Authentication controllers:
     - LoginController - to login
     - LogoutController - to logout
   - Car controllers:
     - AddCarController - to create new car
     - DeleteCarController - to delete car
     - GetAllCarsController - to show all cars
     - AddCarController - to create new car
   - Driver controllers:
     - AddDriverController - to register driver
     - DeleteDriverController - to delete driver
     - GetMyCurrentCarsController - to show all cars of current registered driver
     - GetAllDriversController - to show all drivers
   - Manufacturer controllers:
     - AddManufacturerController - to create new manufacturer
     - DeleteManufacturerController - to delete manufacturer
     - GetAllManufacturersController - to show all manufacturers
   - IndexController - homepage
# Technologies
- **Java 11**
- **Maven 3.8.0 version**
- **JDBC 4.2 version**
- **MySql 8.0.22 version**
- **Java Servlets 4.0.1 version**
- **Apache Tomcat 9.0.65 version**
- **JSTL 1.2 version**
# How to run
- Clone this repository `https://github.com/VitaliiPotseluiko/taxi-service.git`
- Initialize the database by using SQL script : `src/main/resources/init_db.sql`
- Update fields `JDBC_DRIVER`, `URL`, `USERNAME`, `PASSWORD` with your database connection information in `src/main/java/taxi/util/ConnectionUtil.java`
- Build this project using Maven: `mvn clean install`
- Configure run with Tomcat
# Autors
  Vitalii Potseluiko
