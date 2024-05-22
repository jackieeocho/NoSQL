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