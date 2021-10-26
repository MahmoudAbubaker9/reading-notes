# Related Resources and Integration Testing

### Related data in Spring




1. One-to-One Relationship

    A One-to-One (@OneToOne) relationship refers to the relationship between two entities tables A and B in which only one element of A may only be linked to one element of B, and vice versa.

    * We must be careful to have different names for each association resource

2. One-to-Many Relationship

    A One-to-Many (@OneToMany) relationship refers to the relationship between two entities A and B in which one element of A may only be linked to many elements of B, but a member of B is linked to only one element of A.

3. Many-to-Many Relationship

    A Many-to-Many (@ManyToMany) refers to a record in one entity can be referenced by multiple records in another entity.


4. Many-to-One Relationship

    A Many-to-One (@ManyToOne) relationship occurs when multiple records in a table are associated with multiple records in another table. For example, a many-to-many relationship exists between customers and products: customers can purchase various products, and products can be purchased by many customers.

### Integration Testing in Spring

* In integration testing all modules of the the software are tested combined.

* It tests only after the completion of all parts.

Writing Integration Tests:

1. Verify View Name.

2. Verify Response Body.

3. Send GET Request With Path Variable.

4. Send GET Request With Query Parameters.

5. Send POST Request.
