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

This is a web application made using C# and .NET5...

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
* Make sure that .NET Software Development Kit 5 has been installed to your local machine.
* Setup MySQL...

Database setup
* Run the following commands in MySQL to set up this project database:
```
CREATE DATABASE firstname_lastname;
USE firstname_lastname;
CREATE TABLE stylists (
  StylistId int(11) NOT NULL AUTO_INCREMENT,
  Name varchar(255) DEFAULT NULL,
  Details varchar(255) DEFAULT NULL,
  PRIMARY KEY(StylistId)
);
CREATE TABLE clients (
  ClientId int(11) NOT NULL AUTO_INCREMENT,
  Name varchar(255) DEFAULT NULL,
  StylistId int(11) NOT NULL DEFAULT '0',
  PRIMARY KEY(ClientId)
);
```

Installation
* Clone this repository to your machine `$ git clone https://github.com/shanole/HairSalon.Solution`
* In the terminal, navigate to the project directory `$ cd HairSalon.Solution/HairSalon`
* Create `appsettings.json` file in `/HairSalon` directory with the following code:
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=<FIRSTNAME_LASTNAME>;uid=root;pwd=<YOUR PASSWORD HERE>;"
  }
}
```
* Compile code by running command `$ dotnet build`
* Run program with command `$ dotnet run` to open webpage on your preferred browser at `http://localhost:5000`

## Schema <a id="schema"></a>

## Known Bugs <a id="bugs"></a>
* None known at this time. If you find one, please don't hesitate to contact me about it!

## License <a id="license"></a>
*[MIT](https://choosealicense.com/licenses/mit/)*

Copyright (c) 2021 Shannon Lee

## Contact Information <a id="contact"></a>
**_Shannon Lee [mailto](mailto:shannonleehj@gmail.com)_**