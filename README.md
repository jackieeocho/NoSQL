## NoSQL
 
#### What is it?

NoSQL, which stands for "Not Only SQL, is a class of database management systems that provide flexible schemas, high performance and horizontal scalability, designed to handle large volumes of unstructured or semi-structured data.

#### Compare SQL to NoSQL
| DATABASE TYPE  | SQL(relational databases)       | NoSQL(non-relational databases)                              |
|----------------|---------------------------------|--------------------------------------------------------------|
| DATA STRUCTURE | Structured data                 | Semi-structured and Unstructured Data                        |
| SCHEMAS        | Fixed schema that is table like | Dynamic schema                                               |
| LANGUAGE       | Structured Query Language(SQL)  | Database dependant but uses a wide range                     |
| SCALABILITY    | Vertically Scalable             | Horizontally Scalable                                        |
| STRUCTURE      | Table-based                     | Range of forms i.e. key-values stores and document databases |


#### What language(s) can be used?
NoSQL is very flexible supports a wide range of languages for programming and querying. For example JSON, JavaScript,Python,Java, C#, Ruby, Scala etc.

#### Example NoSQL Schema design

#### NoSQL is scalable. Explain the concept and some benefits of it. Any negatives?

#### Types of NoSQL Database?
 
## MongoDB

#### What is MongoDB?
MongoDB is an open source NoSQL database management program that stores data records as documents in a flexible BSON(Binary JSON) format, these are gathered together in collections. It is designed to handle large volumes of unstructured or semi-structured data, offering high performance, scalability, and ease of use, and uses collections and documents, providing more flexibility in data storage and retrieval.

#### What are collections and documents in Mongo? 
A collection is a grouping of MongoDb documents(a basic unit of data) and is the equivalent of a table in a relational database system, a collection exist within a single database. A NoSQL Database contains a collection, and a collection contains documents and the documents contain data, they are related to each other. 

#### MongoDB Architecture, how does it work? 

#### What are replica sets?
A replica set in MongoDB is a group of mongoDB processes that maintain the same data set. Replica sets provide redundancy and high availability, and are the basis for all production deployments. 

#### What is sharding?
Sharding is a method for distributing data across multiple machines/servers to support high volume operations, it is the key feature of horizontal scaling(dividing up a large database ond allocating the shards to smaller servers, this spreads the load, making it more efficient and powerful).

#### Advantages of MongoDB?

#### Disadvantages of MongoDB?

#### What scenarios is MongoDB good for?

#### What scenarios is it not good for?


## MONGOBD EXERCISES

#### Exercise 1

#### Create a collection to store information about your favourite films. Add appropriate validation rules, then insert at least 3 documents. Practice using both .insertOne() and .insertMany(). You may want to type commands into a text editor then paste into the shell.

Create database: The 'use db' command to create a database
```
use myfavouritefilms
```

Store Film information(create collection of documents): The 'db.database.insertMany()' is used to insert the documents into the database.
```
db.myfavouritefilms.insertMany([{
  title: "Tangled",
  director: "Nathan Greno, Byron Howard",
  length: 100,
  company: "Walt Disney Animation Studios"
  },
  {
    title: "High School Musical",
    director: "Kenny Ortega",
    length: 98,
    company: "Disney Channel Original Movies"
  },
  {
    title: "Starstruck",
    director: "Michael Grossman",
    length: 81,
    company: "Disney Channel Original Movies"
  }
])
```

#### Exercise 2

#### Add a new document to the collection, add a new field to that document, remove that field and then remove the document entirely.

Adding Frozen to the collection: The 'db.database.insertOne' command is used to add the Frozen document to the collection.
````
db.myfavouritefilms.insertOne({
  title: "Frozen",
  director: "Chris Buck, Jennifer Lee",
  length: 102,
  company: "Walt Disney Animation Studios"
})
````

Adding a the year of the movie release as a new field in the frozen document: The 'db.database.updateOne' command and '$set' notation is used to add to the database.
````
db.myfavouritefilms.updateOne(
  { title: "Frozen" },
  { $set: {Year: 2013 } }
)
````

Removing the newly added 'Year' field: The 'db.database.updateOne' command and '$unset' notation is used to delete from the database.

````
db.myfavouritefilms.updateOne(
  { title: "Frozen" },
  { $unset: {Year: "" } }
)
````

Deleting the newly added Frozen document: The 'db.database.deleteOne' command is used to remove and delete the specified document from the collection
````
db.myfavouritefilms.deleteOne({ title: "Frozen" })
````
## STAR WARS FILES 

#### Exercise 5

#### Write a query that finds the Luke Skywalker document

#### Return the value of name and eye_colour only, from the "chewbacca" document

#### Find a way to check the species name of admiral ackbar, this is in an embedded document ("Species")



#### Exercise 6 

#### Write a query that gives us only the names + homeworld names of humans in the database?



#### Exercise 7

#### Write a query that gives us all the entries that have an eye_colour of either "yellow" or "orange"



#### Exercise 8

#### You can combine filters using $and or $ or write a query that filter for characters that have both blue eyes and are female.Then write a query that filters for characters that have either blue eyes or are female



#### Exercise 8

#### You can use comparison operators in your queries

#### Write a query that finds characters with a height over 200cm

#### Note, Height has been recorded as a string and there are some missing a height value entirely. Can you find out how to convert all the height strings to ints?

#### Run your initial height query again to confirm your solution works.



#### Exercise 9

#### Experiment with the following operators. What does each do?

$eq
$gt
$gte
$in
$lt
$lte
$ne
$nin


