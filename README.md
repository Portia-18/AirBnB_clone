Contents:
Project Description
General Objetives
Command Interpreter Description
How to start it
Commands and their usage
How to use it
examples
Unittests
Project Description
Airbnb Clone is the main project of the second trimester at Holberton School. The aim is to develop an entire web application that simulates the behavior of the Airbnb platform. Starting from the console or command interpreter, to manipulate data without a visual interface, like in a Shell (perfect for development and debugging), followed by the construction of a website (the front-end) that shows the final product to everybody: static and dynamic, once it's finished what follows is the connection with the database or files that store data (data = objects). And last but not least, the creation of an API that provides a communication interface between the front-end and your data (retrieve, create, delete, update them).

General Objetives
How to create a Python package
How to create a command interpreter in Python using the cmd module
What is Unit testing and how to implement it in a large project
How to serialize and deserialize a Class
How to write and read a JSON file
How to manage datetime
What is an UUID
What is *args and how to use it
What is **kwargs and how to use it
How to handle named arguments in a function
Command Interpreter Description
How to start it

Follow the instructions to get a copy of the program and run in your local machine:

Clone the following repository. https://github.com/HibeeK/AirBnB_clone.git

Run the program ./console.py

How to use it
the console will display a prompt (hbnb) indicating that the user can write and execute a command. After the command is run, the prompt will appear again a wait for a new command

examples
quit or EOF	Exits the program
Usage	By itself
-----	-----
help	Provides a text describing how to use a command.
Usage	By itself --or-- help <command>
-----	-----
create	Creates a new instance of a valid Class, saves it (to the JSON file) and prints the id. Valid classes are: BaseModel, User, State, City, Amenity, Place, Review.
Usage	create <class name>
-----	-----
show	Prints the string representation of an instance based on the class name and id
Usage	show <class name> <id> --or-- <class name>.show(<id>)
-----	-----
destroy	Deletes an instance based on the class name and id (saves the change into a JSON file).
Usage	destroy <class name> <id> --or-- .destroy()
-----	-----
all	Prints all string representation of all instances based or not on the class name.
Usage	By itself or all <class name> --or-- <class name>.all()
-----	-----
update	Updates an instance based on the class name and id by adding or updating attribute (saves the changes into a JSON file).
Usage	update <class name> <id> <attribute name> "<attribute value>" ---or--- <class name>.update(<id>, <attribute name>, <attribute value>) --or-- <class name>.update(<id>, <dictionary representation>)
-----	-----
count	Retrieve the number of instances of a class.
Usage	<class name>.count()
