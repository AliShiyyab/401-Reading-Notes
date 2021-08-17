# Spring Security

1. All of the principles apply equally well to applications that do not use Spring Boot.
2. **Authentication** : The main strategy interface for authentication is AuthenticationManager

>*AuthenticationProvider* : **has an extra method to allow the caller to query whether it supports a given Authentication**

* Spring Security provides some configuration helpers to quickly get common authentication manager features set up in your application AuthenticationManagerBuilder

`authorization` :what are you allowed to do? 

>access control

Core strategy in authorization is AccessDecisionManager.

`AuthenticationException` is a runtime exception ,depending on the style or purpose of the application

## Web Security

>*The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI.*

> Full Describe

* Relation between *Client* <-> *filter* <-> *filterChainProxy* <-> *Filter* <-> *ServLet*.
* all of them mentioned related with Spring Security Filtters.

>**Principal** : used to validate the authentication, so this can be a useful little trick to get a type-safe reference to your user data.