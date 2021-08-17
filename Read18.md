# Many To Many Relation

>**Is the relation between tow tables related with many record in the first table with many record in the other tables.**

>Example : Reltion between customer and products ( customer need many products and products used by many customer )

    @ManyToMany(cascade = { CascadeType.ALL })
    @JoinTable(
    name = "Employee_Project",
    joinColumns = { @JoinColumn(name = "employee_id") },
    inverseJoinColumns = { @JoinColumn(name = "project_id") }
    )
    Set<Project> projects = new HashSet<>();

>In Java used the relation between two models`Entity`.

## Like:

    @Entity
    @Table(name = "Customer")
    public class Customer { @ManyToMany .:.:.}

    @Entity 
    @Table(name= "Products")
    public class products{ @ManyToMany .:.:.}
