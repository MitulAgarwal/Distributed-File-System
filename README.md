# Distributed-File-System
Project based on distributed systems

This project is a Python implementation of a distributed file system. A distributed file system is 
one that enables several users to access and store files on various real or virtual computers. In 
this project, we constructed a system for creating, deleting, and updating files over a network of 
networked computers. Clients can connect to any of the servers in the network to execute file 
operations. File replication is also included in the project to provide data redundancy. This 
project's goal is to create a scalable and dependable file system that can be utilised in a variety 
of applications such as cloud computing, data processing, and storage.4

The key requirements for the project were to create a system that would
Support transparency and data replication.
In the implementation of the project we have used python3 and created multiple server programs 
to which a client can connect to using socket programming.
The project also uses a leafpad editor to read and write documents.
The project allows a user to create, update, delete and list the files created on the server. The 
server then replicates these files on creation and keeps track of them using a global list. The 
main server makes sure that all the files are updated, created, and deleted across the network 
simultaneously, thus, the user can access and edit the documents even if one of the servers 
fails. ls. Thus, the project achieves many core Distributed Systems concepts like data replication, 
data transparency and some fault tolerance.
Features: -
• Create file
• Update file
• Delete file
• List file
In the project we have used one client that connects to one server, however there are three 
servers connected to each other, the client connects to only one of them. Upon connecting to the 
server, the user can implement the above-mentioned features. The server that it is connected to 
updates the global list of files and sends the file for replication creation of the file created.
Upon updating the file, the global list is updated by the main server which then sends another 
request to update the files in consecutive servers by updating the global list. The same 
procedure is followed for the deletion of a file
Whenever any server goes down, the client reconnects to the other server and can still access 
the data created because of data replication and perform the above-mentioned

Client Commands :-
• help
• read <file_name> 
• write <file_name> 
• create <file_name> 
• delete <file_name>
• list 
• exit

