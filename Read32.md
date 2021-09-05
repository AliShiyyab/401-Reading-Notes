# Serverless and Amplify

# Serverless?

>**Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers**

>**Cloud Provider**

* IBM Open Whisk
* AWS Lambda
* Azure Functions
* Google Clouds Functions
* Auth0 Web Tasks

>**Traditional Architecture Helping user to create DataBase, BackEnd Server, FrontEnd UI and Authintication and Authorization Security**

## The Serverless App

>**A Serverless solution consists of a web server, Lambda functions (FaaS), security token service (STS), user authentication and database.**

* **Client Application** — The UI of your application is rendered client side in Modern Frontend Javascript App which allows us to use a simple, static web server.
* **Web Server** — Amazon S3 provides a robust and simple web server. All of the static HTML, CSS and JS files for our application can be served from S3.
* **Lambda functions (FaaS)**— They are the key enablers in Serverless architecture. Some popular examples of FaaS are AWS Lambda, Google Cloud Functions and Microsoft Azure Functions.
* **Security Token Service (STS)** — generates temporary AWS credentials (API key and secret key) for users of the application.
* **User Authentication**— AWS Cognito is an identity service which is integrated with AWS Lambda. With Amazon Cognito, you can easily add user sign-up and sign-in to your mobile and web apps.
* **Database** — AWS DynamoDB provides a fully managed NoSQL database.

## Benifites From Developer Side

* Reduced liability, no backend infrastructure to be responsible for.
* Zero system administration.
* Easier operational management.
* Fosters adoption of Nanoservices, Microservices, SOA Principles.
* Faster set up.
* Scalable, no need to worry about the number of concurrent requests.
* Monitoring out of the box.
* Fosters innovation.

## Benifites From User Side

* If businesses are using that competitive edge to ship features faster, then customers are receiving new features quicker than before.
* It is possible that users can more easily provide their own storage backend(i.e Dropbox, Google Drive).
* It’s more likely that these kinds of apps may offer client-side caching, which provides a better offline experience.

# Amplify

>**AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications,**

>*you can configure app backends and connect your app in minutes*

## Benefits

* Configure backends fast
* Seamlessly connect frontends
* Deploy in a few clicks
* Easily manage content

