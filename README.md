0x00. AirBnB clone - The console
================================
Creation of a command interpreter to manage the hbnb projects

![image](https://github.com/tiztaw/AirBnB_clone/assets/118044736/a8f8e3c7-7349-4ff7-95b9-dd1a970796e8)

Description of the project
===========================

This is the first step towards building your first full web application: the AirBnB clone. The aim of the project is to deploy a replica of the Airbnb Website using my server. The final version of this project will have:
A command interpreter to manipulate data without a visual interface, like a shell (for development and debugging)
A website (front-end) with static and dynamic functionalities
A comprehensive database to manage the backend functionalities
An API that provides a communication interface between the front and backend of the system.
  
Resources
=========
Videos showing examples of how various parts of the project work, listed below:
HBNB videos
Holberton Airbnb overview
The Airbnb Console
Airbnb ORM
Airbnb API
Final product
Other resource
cmd module
	packages concept page
	Python packages
	uuid module
	datetime
	unittest module
	args/kwargs
	Python test cheatsheet
	AirBnB website.

Aims & Objectives of this project
=================================
This will help to be able to manage the objects of our project:
	Creation of a new object (ex: a new "User" or a new "Place")
	Retrieval of an object from a file storage, a database etc… 
	Perform operations on objects (count, compute stats, etc…)
	Update attributes of an object
	Destroy an object

The created objects
===================
The list of the objects (instances) that can be created are as follows:
	BaseModel
	User
	City
	Amenity
	State
	Review
	Place

Files and Directories
=====================
	models directory contains all classes used for the entire project. A class,called “model” in a OOP project is the representation of an object/instance.
	tests directory contains all unit tests.
	console.py file is the entry point of our command interpeter.
	models/base_model.py file is the base class of all our models. It contains common elements:
		attributes: id, created_at and updated_at
		methods: save() and to_json()
models/engine directory contains all storage classes (using the same prototype).
For the moment I will have only one: file_storage.py.

The project's implementation will happen in the following phases:

Phase One
========
The first phase is to manipulate a powerful storage system to give an abstraction between objects and how they are stored and persisted. To achieve this, I will:

	put in place a parent class (called BaseModel) to take care of the initialization, serialization and deserialization of my future instances
	create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file
	create all classes used for AirBnB (User, State, City, Place…) that inherit from BaseModel
	create the first abstracted storage engine of the project: File storage.
	create all unittests to validate all our classes and storage engine
	Create a data model
	Manage (create, update, destroy, etc) objects via a cosole/command interpreter
	Store and persist objects to files (JSON files) 
  
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
(hbnb) 
(hbnb) quit
$
But also in non-interactive mode: (like the Shell project in C)

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
  
Authors
================
  Tiztaw Tsehay and 
  
  Mekuriaw Chekol
