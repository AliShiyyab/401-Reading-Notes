# Working with Relationships in Spring Data REST

## One to One Relations

>**Data Model**

* define two entity classes Library and Address
* have a one to one relation
* using the @OneToOne annotation
* The association is owned by the Library end of the association

*First one :* 

    @Entity
    public class Library {

        @Id
        @GeneratedValue
        private long id;

        @Column
        private String name;

        @OneToOne
        @JoinColumn(name = "address_id")
        @RestResource(path = "libraryAddress", rel="address")
        private Address address;
        
        // standard constructor, getters, setters
    }

*Secone method*

    @Entity
    public class Address {

        @Id
        @GeneratedValue
        private long id;

        @Column(nullable = false)
        private String location;

        @OneToOne(mappedBy = "address")
        private Library library;

        // standard constructor, getters, setters
    }

>**We must be careful to have different names for each association resource**

## The Repositories

In order to **expose these entities as resources**, let's create two repository interfaces for each of them, by extending the CrudRepository interface:

>`public interface LibraryRepository extends CrudRepository<Library, Long> {}`

>`public interface AddressRepository extends CrudRepository<Address, Long> {}`

>Type of **Relations**:

* 1:1
* 1:M
* N:M
* M:1

**and of these mentioned is related between two tables.**