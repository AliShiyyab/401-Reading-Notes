# Spring RESTful Routing & Static Files

## Spring RequestMapping

>In this tutorial, we'll focus on one of the main annotations in **Spring MVC: @RequestMapping**.

## @RequestMapping using paht

>Example

    @RequestMapping(value = "/ex/foos", method = RequestMethod.GET)
        @ResponseBody
        public String getFoosBySimplePath() {
            return "Get some Foos";
        }

## @RequestMapping - the HTTP method :

>Example

    @RequestMapping(value = "/ex/foos", method = POST)
        @ResponseBody
        public String postFoos() {
            return "Post some Foos";
        }

## @RequestMapping With the headers Attribute :

>Example :


    @RequestMapping(value = "/ex/foos", headers = "key=val", method = GET)
    @ResponseBody
    public String getFoosWithHeader() {
        return "Get some Foos with Header";
    }

### Multible Header

>Example

    @RequestMapping(value = "/ex/foos/{fooid}/bar/{barid}", method = GET)
        @ResponseBody
        public String getFoosBySimplePathWithPathVariables
        (@PathVariable long fooid, @PathVariable long barid) {
            return "Get a specific Bar with id=" + barid + 
            " from a Foo with id=" + fooid;
        }

## Access data with JPA:

>Example :

    package com.example.accessingdatajpa;

    import javax.persistence.Entity;
    import javax.persistence.GeneratedValue;
    import javax.persistence.GenerationType;
    import javax.persistence.Id;

    @Entity
    public class Customer {

      @Id
      @GeneratedValue(strategy=GenerationType.AUTO)
      private Long id;
      private String firstName;
      private String lastName;

      protected Customer() {}

      public Customer(String firstName, String lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
      }

      @Override
      public String toString() {
        return String.format(
            "Customer[id=%d, firstName='%s', lastName='%s']",
            id, firstName, lastName);
      }

      public Long getId() {
        return id;
      }

      public String getFirstName() {
        return firstName;
      }

      public String getLastName() {
        return lastName;
      }
    }

