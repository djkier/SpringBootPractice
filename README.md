
# Spring Boot Practice
This repository contains my practice with **Spring Boot** as I learn its core features and functionalities. I'm following the tutorial video **[“Building web applications in Java with Spring Boot 3 – Tutorial”](https://www.youtube.com/watch?v=31KTdfRH6nY)** by **[@Dan Vega](https://github.com/danvega)** , which provides a step-by-step guide to building and understanding Spring Boot applications. Throughout this project, I'll be documenting key concepts, code implementations, and any challenges I encounter as I explore dependency injection, REST APIs, data persistence, and more. Each commit represents a new learning milestone, with updates to both the code and my understanding of Spring Boot.

# Development Environment
-   **IDE:** IntelliJ IDEA
-   **Java Version:** Java 21
-   **Spring Boot Version:** 3.4.4
- **Build Tool:** Maven

# Features Learned
- **`mvn spring-boot:run`** runs the Spring Boot application with all the Spring setup (including annotations and dependency injection), whereas **`mvn exec:java`** is for standard Java programs without Spring Boot’s special configuration.

- **Spring Boot annotations** like `@SpringBootApplication`, `@RestController`, and `@Component` are special keywords we put above classes or methods in a Java program to tell the Spring Boot framework how to treat them. On their own, these annotations don’t do anything, Java by itself doesn’t understand them. But when we use Spring Boot, it looks at these annotations and sets up the program based on what they mean. For example, let say in a kitchen with a lot of different spoons we can't tell their uses but we can know their use if there is a label on it, just like in Spring Boot annotations is like a labels that guide Spring Boot to build and run the application correctly behind the scenes.

- **`@SpringBootApplication`** marks the main class of a Spring Boot application. It tells Spring Boot to start the application, initialize configuration, enable component scanning, and apply default settings.
- **`public static void main(String[] args) {  
    SpringApplication.run(ApplicationName.class, args);  
}`** When you compile a Java application, the JVM looks for the `main` method as the entry point. Inside the `main` method, `SpringApplication.run(ApplicationName.class, args)` is called, which initializes the Spring Boot framework. It processes the `ApplicationName.class` to find configuration annotations like `@SpringBootApplication` and sets up the application context, including auto-configuration and beans. The `args` parameter is passed to Spring Boot, allowing you to handle command-line arguments. Essentially, Spring Boot is started through this line, and the application begins running with all the necessary configurations applied.

