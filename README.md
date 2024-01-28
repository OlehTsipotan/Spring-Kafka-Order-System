# Spring Kafka Order System

----
***Work in progress...***

----

This is a basic example of a microservice architecture using Spring Boot, Spring Kafka (Avro), and Docker. 
The project consists of three microservices: Order Service, Payment Service, and Stock Service. 
All microservices are independent of each other and communicate with each other using Apache Kafka.

## Table of Contents
- [Project Description](#project-description)
- [Technology Stack](#technology-stack)
- [How to Install and Run the Project](#how-to-install-and-run-the-project)
- [Credits](#credits)

## Project Description
The Spring Kafka Order System is designed to provide a flexible and robust API for creating orders and processing their payments, stock. 
Despite all the simplicity of the project, it is designed to be easily scalable and extensible. 
The project is based on the microservice architecture and uses the Apache Kafka message broker and Apache Avro Schema Registry to communicate between microservices. The project is containerized using Docker and can be easily deployed to any cloud platform.
And one of the main intentions of this project is to show how to use Apache Kafka with Avro serialization in Spring Boot applications.

## Technology Stack

- **Backend**:
    - [Java](https://www.java.com/) - A general-purpose programming language that is class-based, object-oriented, and designed to have as few implementation dependencies as possible.
    - [Spring Framework](https://spring.io/) - An application framework and inversion of control container for the Java platform.
        - [Spring Boot](https://spring.io/projects/spring-boot) - An extension of the Spring framework that simplifies the process of building production-ready applications.
        - [Spring Web](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html) - Provides key web-related features, including multipart file upload functionality and initialization of the IoC container.
        - [Spring Data JPA](https://spring.io/projects/spring-data-jpa) - Provides a simple and consistent programming model for data access.
        - [Spring MVC](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html) - The web module of the Spring framework that simplifies the work needed to develop web applications.
        - [Spring Kafka](https://spring.io/projects/spring-kafka) - Provides a KafkaTemplate to send messages to Kafka topics, a listener container for asynchronous consumption of messages, and a listener container for synchronous consumption of messages.
    - [PostgreSQL](https://www.postgresql.org/) - An open-source relational database system.
    - [SpringDoc](https://springdoc.org/) - Library helps to automate the generation of API documentation using spring boot projects
    - [Spring Kafka](https://spring.io/projects/spring-kafka) - Provides a KafkaTemplate to send messages to Kafka topics, a listener container for asynchronous consumption of messages, and a listener container for synchronous consumption of messages.
    - [Apache Avro](https://avro.apache.org/) - A data serialization system.

- **Testing**:
    - [Mockito](https://site.mockito.org/) - Mockito is a mocking framework that tastes really good.
    - [JUnit 5](https://junit.org/junit5/) - A programming and testing model for Java applications.
    - [Testcontainers](https://www.testcontainers.org/) - Provides throwaway instances of common databases, Selenium web browsers, or anything else that can run in a Docker container.
    - [Flyway](https://flywaydb.org/) - Database migration tool.

- **Development Tools**:
    - [Postman](https://www.postman.com/) - Postman is an API platform for building and using APIs.
    - [Lombok](https://projectlombok.org/) - A Java library that helps to reduce boilerplate code.

- **Containerization and Deployment**:
    - [Docker](https://www.docker.com/) - A platform for developing, shipping, and running applications.

## How to Install and Run the Project
### Prerequisites:

- Installed Docker

### Installing
- Clone the repo

```sh
git clone --recurse-submodules git@github.com:OlehTsipotan/Spring-Kafka-Order-System.git
```

### Running
- Run out the box by Docker Compose
```sh
docker-compose --profile prod up 
```
3. Have fun!
   The application will be accessible at
- http://localhost:8080 **Order Service**
- http://localhost:8082 **Payment Service**
- http://localhost:8083 **Stock Service**

## Credits
Oleh Tsipotan - developer (https://www.linkedin.com/in/oleh-tsipotan/)
