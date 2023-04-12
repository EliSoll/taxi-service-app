
[![LinkedIn][linkedin-shield]][linkedin-url]

<div align="center"><h1><img src="https://cdn-icons-png.flaticon.com/512/1183/1183669.png" alt="Logo" width="140" height="90">Taxi Service</h1></div>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built with</a></li>
      </ul>
    </li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#structure">Structure</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>

## About The Project

Taxi service is an application for drivers with basic functionality for users written in Java. It uses Java Servlets (JSP, JSTL), JDBC and SQL. In this project used N-tier architecture with DB layer, DAO layer, Service layer, Controllers layer, Filters. Project was developed according to SOLID principles with possibility of user's authentication.

### Built with:

* Java v.11.0.17
* Java Servlets v.4.0.1
* JDBC v.4.2
* Tomcat v.9.0.73
* Maven v.3.8.0
* MySql v.8.0.22

<div align="center"><a href="https://ibb.co/nkKt6Gz"><img src="https://i.ibb.co/YjVwPCp/demo-app-screen-readme-git.jpg" alt="demo-app-screen-readme-git" border="0"></a></div>

## Getting Started

To get a local copy up and running follow these simple steps:
1. Clone this repository.
2. Download and install the JDK, servlet container (Apache Tomcat or other).
3. Download and install MySQL Server and optional - MySQL Workbench.
4. Create the schema and tables in MySql. Use data from src/main/resources/init_db.sql.
5. Configure ```URL```, ```USERNAME```, ```PASSWORD``` and ```JDBC_DRIVER``` properties with the corresponding values for your DB's connection.
6. Build the project using Maven: 
 ```sh
  mvn clean install
  ```
7. Deploy the WAR file to Tomcat. 

## Structure

 <ol>1. Controllers:
  <ul>1. LoginController - authentication of users.</ul>
  <ul>2. LogoutController - log out for users and invalidation of http session.</ul>
  <ul>3. IndexController - homepage of app.</ul>
  <ul>4. AddCarController - adds a new car.</ul>
<ul>5. AddDriverToCarController - adds a driver to car by carID.</ul>
<ul>6. DeleteCarController - deletes certain car.</ul>
<ul>7. GetAllCarsController - views all cars.</ul>
<ul>8. AddDriverController - adds a driver.</ul>
<ul>9. DeleteDriverController - deletes driver.</ul>
<ul>10. GetAllDriversController - views all drivers.</ul>
<ul>11. GetMyCurrentCarsController - views all cars for the current driver.</ul>
<ul>12. AddManufacturersController - adds new manufacturer.</ul>
<ul>13. DeleteManufacturerController - deletes manufacturer.</ul>
<ul>14. GetAllManufacturersController - views all manufacturers.</ul></ol>

2. DAO Layer: DAOt interfaces with implementations.

3. Filter: Servlet Filters used to pre- and postproccesing requests and responses.

4. Model: data from app.

5. Service layer: Service interfaces with implementations that perform business logic.

6. Util: Utility classes. 

7. Resources: db's scripts, config files.

8. Webapp: CSS, JSP pages.

9. WEB-INF: config files for the web application.

10. Views: all JSP files used as views in the application with css style file.

## Features
1. User's authentication and log out.
2. Create a new car's manufacturer with name and country and delete it.
3. Create a new car with model, manufacture's ID and delete it.
4. Create and delete drivers. 
5. Update drivers with new licence number and name.
6. Add drivers to specific cars by ID.
7. View list of all car/drivers/manufacturers.
8. View all cars belonging to the authenticated driver.

## Contact

Elvira Solnyshkina - elvira.solnyshkina@gmail.com

LinkedIn: [linkedin.com/in/elvira-solnyshkina](https://www.linkedin.com/in/elvira-solnyshkina-232958117/)
<div align="right"><img src="https://i.ibb.co/cJyzyTZ/629b7b077c5cd817694c3233.png" alt="Logo" width="180" height="60">

Project Link: [EliSoll/taxi-service-app](https://github.com/EliSoll/taxi-service-app)</div>
<p align="right">(<a href="#readme-top">back to top</a>)</p></div>

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/elvira-solnyshkina-232958117/
