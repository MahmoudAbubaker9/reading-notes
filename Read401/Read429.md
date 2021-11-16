# Room

### Saving data with Room

* The benefit of apps that are handling non-trivial amounts of structured data is that user can carryon utilizing the app while it's offline, because statistics is locally stored.

* There is a Room persistence library that we can use to access data in SQLite.

Room provides the following benefits: :

1. Compile-time verification of SQL queries.
2. Clear comments or annotations to prevent and reduce errors.
3. Streamlined database migration paths.

**There are three major components in Room:**

1. The database class: it is a class that holds all database and serves.
2. Data Entities that represent tables in database class.
3. Data access objects (DAOs) that holds the methods that are related to database and its statements.

**Database**

AppDatabase defines the database configuration and serves as the app's main access point to the persisted data.

1. The class must be annotated with a @Database

2. The class must be an abstract class that extends RoomDatabase.

3. Define an abstract method that has zero arguments and returns an instance of the DAO class.

```
@Database(entities = {User.class}, version = 1)
public abstract class AppDatabase extends RoomDatabase {
    public abstract UserDao userDao();
}
```

### Defining data using Room entities 

* You define each Room entity as a class that is annotated with @Entity.

* A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

* Each table has a primary key that can be set using @PrimaryKey annotation.

* @Ignore annotation is to ignore fields.

* full-text is for search for details in your database’s tables.
 
* @AutoValue annotation can be used if there are two instances of an entity are equal.

* Room uses the class name as the database table name,

* tableName property of the @Entity annotation an @ColumnInfo annotation to set the name of the column.


### Related entities in Room

In Room there are two ways to define and query a relationship between entities:

1. model the relationship using either an intermediate data class with embedded objects
2. a relational query method with a multimap return type.

**Relations:**

1. one-to-one
2. one-to-many
3. many-to-many

@Relation annotation, parentColumn and entityColumn to set the relation between entities.


### Accessing data using Room DAOs

* DAO can be either an interface or an abstract class, by useing @Dao annotation.
* DAO is used to ease the test of your app while you mock database.

**There are two types of DAO methods that define database interactions:**

1. Convenience methods that let you @insert, @update, and @delete rows in your database.

2. Query methods that let you write your own SQL query to interact with the database.

**************
[Saving data with Room](https://developer.android.com/training/data-storage/room)

[Defining entities in Room](https://developer.android.com/training/data-storage/room/defining-data)

[Related entities in Room](https://developer.android.com/training/data-storage/room/relationships)

[Accessing data with Room](https://developer.android.com/training/data-storage/room/accessing-data#java)
**************