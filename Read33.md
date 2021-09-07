# GraphQL Connection :

## @connection : 
The @connection directive enables you to specify relationships between @model types. Currently, this supports one-to-one, one-to-many, and many-to-one relationships. You may implement many-to-many relationships using two **one-to-many** connections and a joining `@model`.

## Has One

>**Example :** 

    type Project @model {
    id: ID!
    name: String
    team: Team @connection
    }

    type Team @model {
    id: ID!
    name: String!
    }

## Has Many

>**Example**

    type Post @model {
    id: ID!
    title: String!
    comments: [Comment] @connection(keyName: "byPost", fields: ["id"])
    }

    type Comment @model
    @key(name: "byPost", fields: ["postID", "content"]) {
    id: ID!
    postID: ID!
    content: String!
    }

## Many-to-Many connections :

>**Example :** 

    type Post @model {
    id: ID!
    title: String!
    editors: [PostEditor] @connection(keyName: "byPost", fields: ["id"])
    }


## Limit : 

>**The default number of nested objects is 100. You can override this behavior by setting the limit argument. For example:**

    type Post @model {
    id: ID!
    title: String!
    comments: [Comment] @connection(limit: 50)
    }

    type Comment @model {
    id: ID!
    content: String!
    }