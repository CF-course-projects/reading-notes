# Spring RESTful Routing & Static Files

## Accessing Data with JPA
- Define an Entity
  - Use the *@Entity JPA* annotation to mark database entities
  - When a *@Table annotation* is not specified, the class name is used as the default table name
  - The Object's id property is annotated with *@Id* so that JPA understands that it is the object's id
    - The id property is also annotated with the @GeneratedValue annotation to indicate that the ID should be generated automatically
  - Note that if the instance variables are not public you will need getters/setters for the class
- Create Simple Queries
  - To make queries, create an interface that extends JPA repository
    - Syntax: public interface \<className> extends JPArepository\<class, long>
    - By extending the JPAreposity, the class repository inherits methods for persistence. 
    - Spring data JPA also allows the creation of query methods by declaring their method signature
## Baeldung: Comparing Repositories
  - Spring Data Repositories
    - CrudRepository provides CRUD functionalities
    - PagingAndSortingRepository provides methods to do pagination and sort records.
    - JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch
  - Because of the inheritance relationship, **JpaRepository contains the full API of CrudRepository and PagingAndSortingRepository**.
  - Creating CRUD functions via JPA:
    - The Spring Data Repository will auto-generate the implementation *based on the name* we provide it
``` 
@Entity
public class Product 

{

    @Id
    private long id;
    private String name;

    // getters and setters
}

@Repository
public interface ProductRepository extends JpaRepository<Product, Long> {
    Product findByName(String productName);
}
```

  - Basic CRUD methods available via CrudRepository:
    - save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
    - findOne(…) – get a single entity based on passed primary key value
    - findAll() – get an Iterable of all available entities in database
    - count() – return the count of total entities in a table
    - delete(…) – delete an entity based on the passed object
    - exists(…) – verify if an entity exists based on the passed primary key value

  - Methods available via JpaRepository:
    - findAll() – get a List of all available entities in database
    - findAll(…) – get a List of all available entities and sort them using the provided condition
    - save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
    - flush() – flush all pending task to the database
    - saveAndFlush(…) – save the entity and flush changes immediately
    - deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch
