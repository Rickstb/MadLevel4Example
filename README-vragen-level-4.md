# MadLevel4Example vragen level 4

#1 A singleton pattern is used in the class that defines the database. What is the purpose of this pattern?
A singleton is a design pattern that restricts the instantiation of a class to only one instance. Notable uses include controlling concurrency and creating a central point of access for an application to access its data store. 

#2 Why should you load the data in a background thread?
dan werkt alles sneller

#3 What are the three major components of ROOM and what are their responsibilities?

There are 3 major components in Room:

Database: Contains the database holder and serves as the main access point for the underlying connection to your app's persisted, relational data.

The class that's annotated with @Database should satisfy the following conditions:

Be an abstract class that extends RoomDatabase.
Include the list of entities associated with the database within the annotation.
Contain an abstract method that has 0 arguments and returns the class that is annotated with @Dao.
At runtime, you can acquire an instance of Database by calling Room.databaseBuilder() or Room.inMemoryDatabaseBuilder().

Entity: Represents a table within the database.

DAO: Contains the methods used for accessing the database.

#4 How can you extract the current database so that you can see the table, columns, and data?
getDatabase 
