# Eu Claire's Salon

#### Epicodus Code Review: Database Basics

#### By Shannon Lee

#### _Table of Contents_

1. [Description](#description)
2. [Technologies Used](#technologies)
3. [Setup/Installation Requirements](#setup)
4. [Schema](#schema)
5. [Known Bugs](#bugs)
6. [License](#license)
7. [Contact Information](#contact)


## Description <a id="description"></a>

This is a web application made using C#, .NET5, MySQL, and Entity to track a hypothetical hair salon's clients and stylists. This project demonstrates understanding of Database basics and one-to-many relationships.

## Technologies Used <a id="technologies"></a>

* C#
* .NET 5
* MSBuild
* MSTest
* Entity
* MySQL
* git


## Setup/Installation Requirements <a id="setup"></a>

Setup requirements
* Make sure that .NET Software Development Kit 5 and MySQL have been installed to your local machine.

Database setup
* Run the following commands in MySQL to set up this project database with your own first name and last name for the database name:
```
CREATE DATABASE shannon_lee;
USE shannon_lee;
CREATE TABLE stylists (
  stylistid int(11) NOT NULL AUTO_INCREMENT,
  name varchar(255) DEFAULT NULL,
  details varchar(255) DEFAULT NULL,
  PRIMARY KEY(stylistid)
);
CREATE TABLE clients (
  clientid int(11) NOT NULL AUTO_INCREMENT,
  name varchar(255) DEFAULT NULL,
  stylistid int(11) NOT NULL DEFAULT '0',
  PRIMARY KEY(clientid)
);
```

Installation
* Clone this repository to your machine `$ git clone https://github.com/shanole/HairSalon.Solution`
* In the terminal, navigate to the project directory `$ cd HairSalon.Solution/HairSalon`
* Create `appsettings.json` file in `/HairSalon` directory with the following code:
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=shannon_lee;uid=root;pwd=<YOUR PASSWORD HERE>;"
  }
}
```
* Compile code by running command `$ dotnet build`
* Run program with command `$ dotnet run` to open webpage on your preferred browser at `http://localhost:5000`

## Schema <a id="schema"></a>

![schema design](https://github.com/shanole/HairSalon.Solution/blob/main/hairsalonschema.png?raw=true)

## Known Bugs <a id="bugs"></a>
* None known at this time. If you find one, please don't hesitate to contact me about it!

## License <a id="license"></a>
*[MIT](https://choosealicense.com/licenses/mit/)*

Copyright (c) 2021 Shannon Lee

## Contact Information <a id="contact"></a>
**_Shannon Lee [mailto](mailto:shannonleehj@gmail.com)_**