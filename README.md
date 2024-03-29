The goal of the project is to deploy on your server a simple copy of the AirBnB website.

This is the first part that is composed by an interpreter of command line that saves the data of instances in a JSON file. It is developed in Python language using mainly the class Cmd. This project have implemented into the development the unit tests for its general working, used for this the Unittest framework.

Description of the command interpreter:
How to start it Start the console by executing the 'console.py' file:
./console.py
How to use it The 'prompt (hbnb)' tells you that the console is ready to receive instructions, type the instruction:
(hbnb) 
Example The 'help' command shows all commands available in the console:
(hbnb) help
(The 'help' command is built into Cmd)

Output:

(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  all  create  destroy  help  quit  show  update

(hbnb) 
Our commands:
'EOF': Exit the program.
(hbnb) EOF
vagrant@vagrant-ubuntu-trusty-64:~/AirBnB_clone$ 
'all': Prints all string representation of all instances based or not on the class name.
(hbnb) all
[]
(hbnb) 
Shows empty square brackets when not exist instances created.

'create': Create a new instance.
(hbnb) create BaseModel
Generate an id automatically

(hbnb) create BaseModel
da7baf7d-6cf9-406b-9360-da1620dfd622
(hbnb) 
'update': Updates an instance based on the class name an id by adding or updating attribute.
(hbnb) update BaseModel da7baf7d-6cf9-406b-9360-da1620dfd622 name "Betty"
(hbnb) 
'show': Print the string representation of an instance based on the class name and id.
(hbnb) show BaseModel da7baf7d-6cf9-406b-9360-da1620dfd622
[BaseModel] (da7baf7d-6cf9-406b-9360-da1620dfd622) {'id': 'da7baf7d-6cf9-406b-9360-da1620dfd622', 'updated_at': datetime.datetime(2020, 2, 20, 16, 50, 19, 303808), 'created_at': datetime.datetime(2020, 2, 20, 16, 50, 19, 303779), 'name': 'Betty'}
(hbnb) 
'all': Prints all string representation of all instances based or not on the class name.
(hbnb) all
["[BaseModel] (da7baf7d-6cf9-406b-9360-da1620dfd622) {'id': 'da7baf7d-6cf9-406b-9360-da1620dfd622', 'updated_at': datetime.datetime(2020, 2, 20, 16, 50, 19, 303808), 'created_at': datetime.datetime(2020, 2, 20, 16, 50, 19, 303779), 'name': 'Betty'}", "[BaseModel] (3e33d99d-ae43-4a9c-b2aa-e2c58b2122af) {'id': '3e33d99d-ae43-4a9c-b2aa-e2c58b2122af', 'updated_at': datetime.datetime(2020, 2, 20, 16, 51, 45, 868183), 'created_at': datetime.datetime(2020, 2, 20, 16, 51, 45, 868098)}", "[BaseModel] (6a29fe15-856c-49ab-9774-1637b1f07d8c) {'id': '6a29fe15-856c-49ab-9774-1637b1f07d8c', 'updated_at': datetime.datetime(2020, 2, 20, 16, 51, 55, 606952), 'created_at': datetime.datetime(2020, 2, 20, 16, 51, 55, 606919)}", "[BaseModel] (6ec48ab4-cf1e-44ca-966c-103d454567c2) {'id': '6ec48ab4-cf1e-44ca-966c-103d454567c2', 'updated_at': datetime.datetime(2020, 2, 20, 16, 51, 48, 63180), 'created_at': datetime.datetime(2020, 2, 20, 16, 51, 48, 63146)}"]
(hbnb) 
Now shows all instances created.

'destroy': Deletes an instance based on the class name and id.
(hbnb) destroy BaseModel da7baf7d-6cf9-406b-9360-da1620dfd622
'quit': Exit the program.
(hbnb) quit
