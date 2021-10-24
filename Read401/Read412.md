# Spring RESTful Routing & Static Files

### Spring RequestMapping

* @RequestMapping is one of the most common annotation used in Spring Web applications. This annotation maps HTTP requests to handler methods of MVC and REST controllers.

* The @RequestMapping annotation can be applied to class-level and/or method-level in a controller.

* You can have multiple request mappings for a method. For that add one @RequestMapping annotation with a list of values.


**There are many applications to use RequestMapping**

form more example visit this site [resources ](https://www.baeldung.com/spring-requestmapping)


### Accessing Data with JPA

* JPA is a specification. It is a collection of classes and methods to persistently store the vast amounts of data into a database. 

*  JPA is an abbreviation that stands for Java Persistence API. It's a specification which is part of Java EE and defines an API for object-relational mappings and for managing persistent objects.

**There are many applications to JPA**

form more example visit this site [resources ](https://spring.io/guides/gs/accessing-data-jpa/)

### Baeldung: Comparing repositories

there is different kinds of Spring Data repository interfaces and their functionality :

1. CrudRepository : provides CRUD functions
2. PagingAndSortingRepository : provides methods to do pagination and sort records
3. JpaRepository : It contains the full API of CrudRepository and PagingAndSortingRepository ,So it contains API for basic CRUD operations and also API for pagination and sorting


**CrudRepository**

the typical CRUD functionality is :

1. save
2. findOne
3. findAll
4. count
5. delete
6. exists

**JpaRepository**

the typical CRUD functionality is :

1. findAll() 
2. save
3. flush
4. saveAndFlush
5. deleteInBatch

**PagingAndSortingRepository**

When using Pageable, we create a Pageable object with certain properties and we've to specify at least:

1. Page size
2. Current page number
3. Sorting

**form more information visit this site [resources ](https://spring.io/guides/gs/accessing-data-jpa/)**



