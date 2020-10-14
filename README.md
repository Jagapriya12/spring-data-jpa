# spring-data-jpa
This simple project uses Spring data JPA repository for CRUD operations

URL	Method

- http://localhost:8080/api/employees GET	- to list all the employees in JSON 
- http://localhost:8080/api/employees	POST	Add a person	JSON
- http://localhost:8080/api/employees/{employeeId}	GET	- to display only one employee based on the id	
- http://localhost:8080/api/employees	PUT	Update a employee details	JSON
- http://localhost:8080/api/employees/{employeeId}	DELETE	Delete the specified employee
 
 MySql database sql script to create schema and employee-repository  
 CREATE DATABASE  IF NOT EXISTS `employee_directory`;
USE `employee_directory`;

--
-- Table structure for table `employee`
--

DROP TABLE IF EXISTS `employee`;

CREATE TABLE `employee` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(45) DEFAULT NULL,
  `last_name` varchar(45) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=latin1;

