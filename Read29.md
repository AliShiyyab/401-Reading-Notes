># Save Data in Your Local Database Using the Room Persistence Library

>**This library allows you to perform the create, read, update, and delete operations the same way you would in SQLite API with less verbosity**

## Three major components in Room:

* `Database` 
* `Entity`
* `DAO` : *Contains the methods used for accessing the database.*(**new**)

## Implementation

>We will be creating a very simple table that consists of the following data:

* `UID` — Unique id for the data.
* `Name` — A string column.
* `Timestamp` — The timestamp in full during the insertion.

>Add the following variables:

    @PrimaryKey(autoGenerate = true)  //This decorator sets the current variable as the primary key for the table.
    public int uid;

    @ColumnInfo(name = "timestamp")   // Determines if this value will be auto-incremented.
    public long timestamp;

    @ColumnInfo(name = "name")     //Sets the name of the column to another name.
    public String name;

>**Change the class into an interface and add the following code. I have created more functions to:**

* Get all data from the table.
* Get all rows from the table based on UID.
* Insert rows of data into the table.
* Delete a single row from the table.
* Clear all data in the table.

